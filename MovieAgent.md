# Create a Movie Agent in Azure AI Foundry

This guide walks you through creating a simple **MovieAgent** in Azure
AI Foundry that can answer questions about movies using the **Web Search
tool**.

------------------------------------------------------------------------

## 🟢 Step 1: Create a New Agent

1.  Sign in to **Azure AI Foundry**.
2.  Go to your **Project → Agents → New Agent**.
3.  Fill in the following details:

**Name:**

    MovieAgent

**Model:**

    gpt-35-turbo

*(or `gpt-4` if available)*

**Instructions (System Prompt):**

    You are a helpful agent that answers questions about movies.
    When asked about movie details, use the web search tool to fetch information.

------------------------------------------------------------------------

## 🟢 Step 2: Add the Web Search Tool

1.  In the agent creation screen, scroll to **Tools**.
2.  Click **Add Tool → Web Search**.

Configure the tool:

**Tool Name:**

    search_web

**Description:**

    Search the web for movie details.

> Leave all default settings for Bing Search integration (it is
> built-in).

------------------------------------------------------------------------

## 🟢 Step 3: Save and Test

1.  Click **Save Agent**.
2.  Open the **Playground** tab.
3.  Test the agent with the prompt:

```{=html}
<!-- -->
```
    Tell me about the movie Inception

The agent will automatically call the web search tool and return details
such as: - Cast - Release year - Plot summary - Other relevant movie
information

------------------------------------------------------------------------

## 🟢 Step 4: (Optional) Refine Instructions

You can make the agent more specific by updating its instructions to:

    Always provide movie details including release year, director, main cast, and a short plot summary.

------------------------------------------------------------------------

## ✅ Result

You now have a MovieAgent capable of answering movie-related questions
by using live web search results.
