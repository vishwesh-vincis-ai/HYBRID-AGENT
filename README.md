# Hybrid Agent (Project 2)

One customer memory across WhatsApp text, voice notes and calls.

Status: **not started**. Build order: brain → lead engine → voice agent → **hybrid agent**.

## What it does
- Router → sales / support / booking specialist.
- Per-customer memory (preferences, history, open issues), shared across channels, never across customers.
- Voice-note transcription; Tamil, English and Tanglish.
- Scheduled proactive follow-ups ("you asked about X yesterday").
- Escalation with summary; never re-asks what the customer already answered.

## Depends on Business Brain
`POST /chat` (session_id = customer's WhatsApp number), calendar endpoints, handoffs.

## Stack
LangGraph, WhatsApp Cloud API, model routing (cheap router, strong reasoner), Supabase, job queue.
