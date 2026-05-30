# Gitscope

Gitscope is a real-time Solana dashboard for monitoring GitHub-linked token activity from earliest signal to later validation.

It is built around a simple event sequence:

- Link: a token appears with a GitHub-linked identity
- Lock: the fee route becomes fixed
- Claim: fee movement confirms that the route is active

Gitscope helps traders follow that sequence inside one terminal, inspect signal quality, filter noisy setups, and review historical winners in context.

## Watch the demo

[![Watch the demo](https://img.youtube.com/vi/UdK_8XhNmk4/hqdefault.jpg)](https://youtu.be/UdK_8XhNmk4)

## What it does

- streams live token events in a terminal-style dashboard
- tracks Link, Lock, and Claim signals in separate columns
- enriches events with GitHub profile context
- highlights timing and quality signals inside each card
- helps separate cleaner setups from noisy lock activity
- lets users review historical follow-through in Top Gainers
- includes admin tools for deeper workflow and strategy analysis

## Product flow

The terminal is designed to make one workflow easy to read:

1. catch the earliest GitHub-linked signal
2. watch for route lock confirmation
3. inspect GitHub quality and lock timing
4. use Fade locks to reduce noise
5. treat claims as validation, not earliest entry
6. review historical winners through Top Gainers

## Stack

- FastAPI backend
- Vue 3 frontend
- WebSocket event delivery
- Docker-based deployment
