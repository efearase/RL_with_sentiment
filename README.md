# RL_with_sentiment
The project is part of the course Machine Learning in Finance at ENSAE.
In this project, we are trying to incorporate investors' sentiment data into a portfolio-managing strategy by Reinforcement Learning.

Our approach is based on the absence of institutional investors in the Russian market, and the assumption that the prices are mainly driven by the "retail" investors, who usually share their opinions on social media. To incorporate this data, we used a parser by @meanother (https://github.com/meanother/tpulse-py) to first obtain the posts written by investors on the investment-oriented social network called pulse (https://www.tinkoff.ru/invest/pulse/). Then we measure the profitability of the investor and his number of followers, which we then use to measure the "utility" of the investor. We also use dostoevsky (https://pypi.org/project/dostoevsky/) and DeepPavlov (https://huggingface.co/blanchefort/rubert-base-cased-sentiment/) frameworks to get the sentiment class of the post. After this train the models on the data with some technical features, which could be also used by the investors to make their decisions. 
