---
title: "Evaluate your Amazon Nova Sonic voice agent at scale, no microphone required"
url: "https://aws.amazon.com/blogs/machine-learning/evaluate-your-amazon-nova-sonic-voice-agent-at-scale-no-microphone-required/"
date: "2026-06-08"
author: "Osman Ipek"
feed_url: "https://aws.amazon.com/blogs/machine-learning/feed/"
---
In this post, we walk you through the Nova Sonic Test Harness, an open source framework that we built to solve both problems. It serves as a rapid iteration tool for tuning system prompts and tool configurations (run a conversation, see results, adjust, repeat) and as a comprehensive evaluation framework for validating voice agent quality at scale. It runs complete multi-turn conversations with Amazon Nova Sonic automatically, evaluates them using LLM-as-judge techniques, and can even detect cases where the model’s audio output doesn’t match its text output (audio hallucinations).
