# Feature Requests from Sales Meetings

This repository automatically tracks feature requests mentioned by leads during sales calls.

## How It Works

1. **Automatic extraction**: After each sales meeting on Attio, our system transcribes the call and uses LLM analysis to extract feature requests
2. **Smart grouping**: Features are automatically grouped into thematic sections using AI
3. **Full attribution**: Every feature request includes:
   - Lead name and company
   - Meeting ID and date
   - Importance level (critical/high/medium/low)
   - Context about why they need it

## File Structure

- `FEATURE_REQUESTS.md` - The main list of all feature requests, organized by theme
- `README.md` - This file

## Updates

This repo is automatically updated via Celery task after each meeting summary is generated. Commits are pushed immediately after processing.

## Viewing

Browse `FEATURE_REQUESTS.md` to see all requests. Each section groups related features together, with newest requests appended to the bottom of each section.
