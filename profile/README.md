# Camoufler

> Protect your data before it reaches AI.

Camoufler is an open-source privacy layer between you and AI services.

When we use AI, our messages can contain names, email addresses, phone numbers, addresses, company information, personal stories, and other details that we may not want to share.

Camoufler processes your message locally and helps remove or transform information that can identify you before the message is sent to an AI service.

## Why Camoufler?

AI is useful because it needs context.

But AI doesn't always need to know **who you are**.

For example, you might ask:

> Can you help me write an email to John Smith at john.smith@example.com about our $50,000 project?

Camoufler can transform the message into something like:

> Can you help me write an email to [PERSON] at [EMAIL] about our [AMOUNT] project?

The AI can still help with the task without receiving the original personal information.

## How it works

```text
                 ┌─────────────┐
                 │    User     │
                 └──────┬──────┘
                        │
                        │ Original message
                        ▼
              ┌────────────────────┐
              │     Camoufler      │
              │                    │
              │  Local processing  │
              │  Privacy layer     │
              └─────────┬──────────┘
                        │
                        │ Protected message
                        ▼
                 ┌─────────────┐
                 │     AI      │
                 └─────────────┘
