# Langchain Agent using a regressor as a tool in a commercial real state recommendation system scenario

Simple integration between a regression model working as a apartment price recommendation system and an LLM Agent using langchain. The dataset used contains real state data from India.

Dataset: https://www.kaggle.com/datasets/shudhanshusingh/real-estate-properties-dataset/data

Langchain topics: Tools and Agents

Regressor: Random Forest

# Overview

## Business Undestanding

We are tring to create an Agent to act as an assistant that can help assign valuation price to apartments in India

## Data understanding

We perform an exploratory analisis to better understand the data we are dealing with, that way we can guest the strong and weak points of out dataset. For example, most of the apartments of our dataset are located in Mumbai, which will give us much accurate results for that region, but less accurate results for others. This can help us guide future improvements in the dataset, and thus, our regression model.

## Data preparation

Here we select, clean, construct, integrate and format our dataset for our training.

## Regressor Modeling

We Select and test models, changing is parameters as needed until a satisfactory metric is reached for our regressor. Finally we save our model to a pickle format. 

## Agent Integration

We use LangChain v0.2 to create an agent capable of chatting with the user and, upon user request, said agent can perform a predict an apartment price given some inputs from the user like:

- City where the apartment is located
- Square footage of the apartment
- Whether it has a pool or not 

In order to do that, the agent will use a tool which is a function that structs user information, inputs it to our regressor and finally replies the user with the price prediction.



# Release Notes

## v0.1

Release com todos os passos integrados em um notebook.






