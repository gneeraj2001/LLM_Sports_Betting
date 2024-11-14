This Python bot is designed to fetch NBA game data, analyze betting odds, and generate predictions or detailed analyses for upcoming games. It uses APIs to gather betting odds and LLMs to generate game insights or predictions. This bot is intended for sports enthusiasts or bettors looking for automated insights on NBA games.

*Features*
   Fetches daily NBA game schedules and betting odds.
   Analyzes games to provide predictions or in-depth analysis.
   Logs predictions and saves results to files for historical reference.
   Updates regularly to ensure that predictions are available for games starting soon.


The LLM (Large Language Model) in this bot uses natural language prompts to generate predictions or analyses for NBA games.
   1. Inputs to the LLM
         Game Description: A concise summary of the matchup, including the teams and game time.
      
            -Example: "Bulls vs Knicks"
         Betting Odds: The latest odds data for the game from various bookmakers.
      
            -Example: "Current odds from DraftKings, FanDuel: Knicks: -120, Bulls: +110"
      
         Additional Context:
      
            -For detailed analyses, the bot includes contextual data like:
            -Recent team performance.
            -Player statistics (PPG, RPG, etc.).
            -Head-to-head records.
            -Injuries or significant changes.
            -Team offensive and defensive efficiency.
      
   3. Query Construction
         The bot builds a natural language query tailored to either:

         Prediction:
      
            Asking for a simple winner prediction.
         Detailed Analysis: Requesting a comprehensive breakdown of the game.
         Example Queries:

            -Prediction: "Can you predict the winner for the upcoming game of Bulls vs Knicks?"
            -Detailed Analysis: "Analyze the game: Bulls vs Knicks. Provide insights on recent form, key players, and head-to-head performance. Suggest betting strategies."
   5. Model and Prediction Generation
         The bot uses LLMs like GPT-4 or Claude to process these queries.
         Depending on the query, the LLM generates:
      
            Winner Prediction: Simple result (e.g., "My prediction is: Knicks will win.").
            Detailed Analysis: A comprehensive analysis considering various game factors.
   7. Sources of Information for Predictions:
   8.             Pretrained Knowledge:
               The LLM is trained on a vast dataset, which includes general sports knowledge, historical NBA data, and betting strategies.
            Real-Time Betting Data:
               The odds fetched from APIs provide live, game-specific data that enhance the prediction accuracy.
            User-Provided Context:
               Specific game data (e.g., injuries, performance trends) from the bot’s query.
   9. Output
         The LLM returns a prediction or analysis based on:

            Statistical trends.
            Current odds.
            Context provided in the query.
         Example Output:
      
            My prediction is: Knicks will win.
            Confidence Level: Medium.
            Rationale: The Knicks have a strong home performance and a better defensive rating. However, the Bulls’ recent form suggests it could be a close game.
            Suggested Betting: Money line on Knicks; consider the under for total points.
