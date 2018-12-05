# UNO Bot

Really basic chat bot experiment using [Stealth](https://github.com/hellostealth/stealth).

## Development

### Local Setup

To run you must have a Ruby development environment setup and then must install the `stealth` Gem.

```bash
gem install stealth
```

To run the server locally you must also setup and run Redis:

```bash
brew install redis
redis-server
```

Stealth recommends [utilizing ngrok](https://hellostealth.org/docs/#local_development.introspectable_tunnels_to_localhost) when developing locally.

After [setting up ngrok](https://gist.github.com/wosephjeber/aa174fb851dfe87e644e), you'll run the following:

```bash
ngrok http 5000
```

Which should provide a basic overview of activity/status here: http://localhost:4040/inspect/http

And then finally, start the Stealth server:

```bash
stealth server
```

### Quick Setup

If everything has been installed and setup correctly, the following commands should run successfully and provide and working chat/bat server:

- `redis-server`
- `stealth server`
- `ngrok http 5000` _(Optional)_

Or, for short: `redis-server& && stealth server`.

** Next Steps**

- [ ] Basic setup/UI implementation with [supported service integration](https://hellostealth.org/docs/#messaging_integrations).
- [ ] Provide accompanying repository for chat UI.
- [ ] Vagrant environment for all key components of the development workflow.

## Resources

- Stealth | Local Development [[1]](https://hellostealth.org/docs/#local_development)
- ngrok setup on OS X [[1]](https://gist.github.com/wosephjeber/aa174fb851dfe87e644e)
- Creating a Chatbot with Stealth [[1]](https://medium.com/v%C3%ADdeos-de-ti/parte-1-stealth-crie-chatbots-incr%C3%ADveis-com-ferramentas-que-voc%C3%AA-conhece-e-adora-f46e1f9c6a5c) [[2]](https://medium.com/v%C3%ADdeos-de-ti/desenvolvendo-seu-primeiro-chatbot-utilizando-o-framework-stealth-dbf1be1508c0)
