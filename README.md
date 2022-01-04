CRISP-DM Framework

Business understanding – What does the business need?

    One business such as Spotify that hosts millions of songs needs a way to automatically sort songs by genre. Also, a rock music magazine would want a way
    to automatically find new songs in the genre in order to review them.

Data understanding – What data do we have / need? Is it clean?

    The data we have is statistics taken directly from Spotify. It has all of the metadata of the song, in addition to spotify's own statistics that give more specific info about the song. Most of the features are clean, however the tempo and duration_ms have some missing values that need fixed.

Data preparation – How do we organize the data for modeling?

    The plan for cleaning this data is to replace all missing values with the mean for that column. Then the duplicates will be removed, features with a low variance  will be removed, and the data will be normalized.

Modeling – What modeling techniques should we apply?

    First the dataset will be split into training and testing data. Then I will try modeling it with a multi-layer perceptron classifier, linear regression, K Neighbors classifiers, and a random forest classifier.

Evaluation – Which model best meets the business objectives?

    The multi-layer perceptron was the best model for this problem as it has the highest accuracy score, and very competitive precision and recall scores. It has a longer run-time than other models but as this model only needs to run once per song on upload, accuracy is more important.

Deployment – How do stakeholders access the results?

    This notebook, the results, and the model will be posted on GitHub. After completing this project, I am happy with the amount of cleaning data that I was able to accomplish. One thing I would want to improve in the future is adapt this problem to be multinomial and detect all genres.