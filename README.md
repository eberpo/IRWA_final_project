    # infoRetrieval

    ## Goal
    The goal of this project is to create a **search engine** with a user interface for retrieving relevant tweets and implementing **web analytics** to track and analyze user interactions. 

    This project involves:
    - Designing a search interface for users to input queries and view results.
    - Enhancing the search algorithms for improved performance.
    - Collecting and visualizing web analytics data, such as user behavior, query statistics, and document engagement metrics.


    ## Project Content

        #### a. Search Page
        - A main web page with a central search box and a search button for users to enter their queries.
        #### b. Search Action
        - The entered query is passed to the search engine’s `search` function.
        #### c. Search Function
        - A general `search` function processes the query string and calls ranking algorithm.

        #### d. Results Page
        - The result page displays the ranked list of retrieved documents with the following details:
            - **Title**: Initial substring of the tweet text.
            - **Summary**: Full tweet text.
            - **Creation Date/Time**.
            - **URL**: Links to the detailed document page.
            - **Relevance Metrics**: Additional indicators like likes, retweets.

        #### e. Document Details Page
        - A detailed view of the selected document with additional information from the corpus.

        #### f. Analytics Dashboard
        - A web page for visualizing website usage and search engine performance.
            - Key metrics include:
            - Query frequency.
            - Document clicks.
            - Dwell times.
            - Interactive graphs and explanations.

    ##Ranking Approach used: 
        Custom Score + Cosine Similarity: CustomScore = (α * TF-IDF Score) + (β * Log(Likes + 1)) + (γ * Log(Retweets + 1))
            We can see that if we change alpha beta or gamma the number of common documents changes.
    
    ## Installation and Environment Setup

    ### Prerequisites
    - Python 3.8 or above.
    - Flask web framework.

    
    ## Dependencies and Libraries
    Make sure the following libraries are installed:
    - `indic-nlp-library`
    - `punjabi_stopwords`
    - `LiHiSTO`
    - `emoji`
    - `wordcloud`

    You can install these directly in Colab with the following command:
    ```bash
    !pip install indic-nlp-library punjabi_stopwords LiHiSTO emoji wordcloud


    ## Running
        1. Clone the repository
        2. Enter in search-engine-web-app folder 
        3. to run the application use:
            python web_app.py
        

Find additional information in the report.