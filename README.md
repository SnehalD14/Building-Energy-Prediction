## Energy Prediction

You can use the [editor on GitHub](https://github.com/SnehalD14/Building-Energy-Prediction/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

## Motivation
With passing years, the notion of having tall buildings for using ground space effectively is booming. Although such buildings are effective, it is becoming expensive to regulate their temperatures. Construction companies have introduced some improvements like cool roofs and higher insulations to cut these costs but assessing the value of energy efficiency improvements can be challenging as there's no way to truly know how much energy a building would have used without these improvements. The function of this tool is to predict the energy consumed by a building without any retrofits and motivate large scale investors to witness the usefulness of these improvements. This tool will take into account building specifications(size, year built, number of floors) and weather conditions (air temperature, wind speed, wind direction) to predict the energy consumed without using any energy saving advancements. 

Why would we need such a tool and who would you expect to use it and benefit from it?
Usage of the tool: The purpose of this tool is to predict how much energy a building with certain properties will consume under certain weather conditions. For example, given the age, size, and purpose of the building, the tool could predict the impact of cooling it in the summer. The main usage of such a tool is to incentivize building owners to implement energy-saving improvements, such as higher insulation or using smart Energy Star products. By predicting the energy consumption of the building without the improvements, we can see whether the improvements are working, and reward owners for the higher performance of their building.

Potential users of the tool: Building this tool is currently an open competition set up by ASHRAE, the American Society of Heating, Refrigerating and Air-Conditioning Engineers. For them, this is an opportunity to have more investors interested in the benefits of using their high-tech heating and cooling systems.

Does this kind of tools already exist? If similar tools exist, how is your tool different from them? Would people care about the difference? How hard is it to build such a tool? What is the challenge?
Available tools in the market: The tools available in the market are modeled with high accuracy but for a few types of buildings or behaviors or a specific location. Also, many of the techniques developed are not publicly available to the general research community.

Advantages of our tool: Our tool will be able to comprehensively account for all the different types of buildings or behaviors. This would enable better estimates of energy-saving investments and encourage large scale investors and financial institutions to invest in this area to enable progress in building efficiencies. An open-source and generalized tool would be easy and convenient to use, thus making it a lucrative option for potential customers.




Challenges: One major challenge in this project would be data cleaning and validation. The provided data has several missing values and the features, “date and time” are not mentioned according to the time zone of the location where the data was recorded but it has been standardized to UTC. The data would have to be validated for realistic values, for example, the year the building was made can’t exceed 2019. One other concern would be overfitting the data for a few types of building and underfitting for the others due to a varied dataset.

How do you plan to build it? You should mention the data you will use and the core algorithm that you will implement
Since this problem is an ongoing kaggle competition, we will build the tool using the data ASHRAE has provided. The data have building details i.e. primary use, area, year built and floor count and weather information i.e. air temperature, cloud coverage, dew temperature, wind direction, and wind speed. We must predict a meter reading that depicts the amount of energy consumed by building considering its properties and weather specifications. We will first preprocess the data to select the important features and convert categorical features to numerical if required. After this, we will apply different machine learning algorithms i.e. regression, support vector machines, random forests and artificial neural networks to identify the algorithm which produces the result closest to the current winners.

What existing resources can you use?
There are three resources we are interested in using: data, algorithms,  and computational power. The data is provided by ASHRAE and consists of various building properties and their energy meter readings at certain times of the year. It was collected over a three-year period and seems fairly complete. The algorithms we are interested in are mostly implemented within scikit-learn, though we may attempt to implement a neural network using PyTorch. In this case, basic documentation is our most powerful resource. For computational power, we intend to apply for access to the ACE cluster once we are more clear on our needs and software requirements.

How will you demonstrate the usefulness of your tool?
Since our end product is a model-based tool that predicts the energy consumed by the building, its usefulness can be demonstrated by measuring the number of correct predictions that it makes. We will divide our training data into a training and test set. After training, we will use our model for making predictions on the test sets and count the number of correct predictions. Also, as this is an ongoing kaggle competition, so we will upload our results on kaggle to see where our tool stands in the leaderboard. Kaggle will be using the Root Mean Squared Logarithmic Error (RMSLE) for estimating the efficiency of our prediction on the provided test data.

References:  
 https://www.mdpi.com/2504-4990/1/3/56/htm
 https://www.kaggle.com/c/ashrae-energy-prediction



Note: This project is an ongoing Kaggle competition with the title “ASHRAE - Great Energy Predictor III” and submissions are due by 19th Dec 2019. Further information about the competition can be obtained in the link https://www.kaggle.com/c/ashrae-energy-prediction



### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/SnehalD14/Building-Energy-Prediction/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Snehal Dikhale

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
