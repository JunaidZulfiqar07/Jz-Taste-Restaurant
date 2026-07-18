# JZ Taste Restaurant 🍔
An AI-powered ordering and reservation website for a fast food restaurant concept, featuring a conversational assistant that handles orders, table bookings, and menu inquiries end-to-end — no forms, no manual entry.
## Overview
JZ Taste is a fully responsive restaurant landing page with an embedded AI chat assistant. Customers can place orders or book a table simply by chatting — the assistant collects the required details, logs the order, and sends an automated confirmation email.
## Features
🎨 Custom-designed, responsive landing page (menu, hours, location)
💬 Embedded AI chat widget for orders and reservations
🧠 Conversational AI agent that understands context across a multi-turn chat
📋 Live menu synced from Google Sheets
📧 Automated order confirmation emails via Gmail
📊 Orders logged automatically to a Google Sheet
Tech Stack
Layer
Technology
Frontend
Single-file index.html (inline CSS + vanilla JS)
Hosting
GitHub Pages
Automation / Backend
n8n
AI Model
Cohere (Command)
Chat Widget
@n8n/chat
Data Storage
Google Sheets
Notifications
Gmail API How It Works
Visitor opens the chat widget on the site.
Messages are sent to an n8n webhook, which triggers an AI Agent workflow.
The AI Agent (powered by Cohere) reads the live menu from Google Sheets, gathers order/reservation details across the conversation, and decides when to take action.
Once all required details are collected, the agent logs the order to Google Sheets and sends a confirmation email via Gmail.
## Project Status
🚧 Actively being built and refined — currently focused on improving conversational reliability and session handling.
