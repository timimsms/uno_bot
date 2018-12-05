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

And then finally, start the chatbot server:

```bash
stealth server
```
