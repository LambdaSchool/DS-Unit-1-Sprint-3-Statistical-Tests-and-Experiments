{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "name": "DS Unit 1 Sprint Challenge 4.ipynb",
      "version": "0.3.2",
      "provenance": [],
      "collapsed_sections": []
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    }
  },
  "cells": [
    {
      "metadata": {
        "id": "NooAiTdnafkz",
        "colab_type": "text"
      },
      "cell_type": "markdown",
      "source": [
        "# Data Science Unit 1 Sprint Challenge 4\n",
        "\n",
        "## Exploring Data, Testing Hypotheses\n",
        "\n",
        "In this sprint challenge you will look at a dataset of people being approved or rejected for credit.\n",
        "\n",
        "https://archive.ics.uci.edu/ml/datasets/Credit+Approval\n",
        "\n",
        "Data Set Information: This file concerns credit card applications. All attribute names and values have been changed to meaningless symbols to protect confidentiality of the data. This dataset is interesting because there is a good mix of attributes -- continuous, nominal with small numbers of values, and nominal with larger numbers of values. There are also a few missing values.\n",
        "\n",
        "Attribute Information:\n",
        "- A1: b, a.\n",
        "- A2: continuous.\n",
        "- A3: continuous.\n",
        "- A4: u, y, l, t.\n",
        "- A5: g, p, gg.\n",
        "- A6: c, d, cc, i, j, k, m, r, q, w, x, e, aa, ff.\n",
        "- A7: v, h, bb, j, n, z, dd, ff, o.\n",
        "- A8: continuous.\n",
        "- A9: t, f.\n",
        "- A10: t, f.\n",
        "- A11: continuous.\n",
        "- A12: t, f.\n",
        "- A13: g, p, s.\n",
        "- A14: continuous.\n",
        "- A15: continuous.\n",
        "- A16: +,- (class attribute)\n",
        "\n",
        "Yes, most of that doesn't mean anything. A16 (the class attribute) is the most interesting, as it separates the 307 approved cases from the 383 rejected cases. The remaining variables have been obfuscated for privacy - a challenge you may have to deal with in your data science career.\n",
        "\n",
        "Sprint challenges are evaluated based on satisfactory completion of each part. It is suggested you work through it in order, getting each aspect reasonably working, before trying to deeply explore, iterate, or refine any given step. Once you get to the end, if you want to go back and improve things, go for it!"
      ]
    },
    {
      "metadata": {
        "id": "5wch6ksCbJtZ",
        "colab_type": "text"
      },
      "cell_type": "markdown",
      "source": [
        "## Part 1 - Load and validate the data\n",
        "\n",
        "- Load the data as a `pandas` data frame.\n",
        "- Validate that it has the appropriate number of observations (you can check the raw file, and also read the dataset description from UCI).\n",
        "- UCI says there should be missing data - check, and if necessary change the data so pandas recognizes it as na\n",
        "- Make sure that the loaded features are of the types described above (continuous values should be treated as float), and correct as necessary\n",
        "\n",
        "This is review, but skills that you'll use at the start of any data exploration. Further, you may have to do some investigation to figure out which file to load from - that is part of the puzzle."
      ]
    },
    {
      "metadata": {
        "id": "Q79xDLckzibS",
        "colab_type": "code",
        "colab": {}
      },
      "cell_type": "code",
      "source": [
        "# TODO"
      ],
      "execution_count": 0,
      "outputs": []
    },
    {
      "metadata": {
        "id": "G7rLytbrO38L",
        "colab_type": "text"
      },
      "cell_type": "markdown",
      "source": [
        "## Part 2 - Exploring data, Testing hypotheses\n",
        "\n",
        "The only thing we really know about this data is that A16 is the class label. Besides that, we have 6 continuous (float) features and 9 categorical features.\n",
        "\n",
        "Explore the data: you can use whatever approach (tables, utility functions, visualizations) to get an impression of the distributions and relationships of the variables. In general, your goal is to understand how the features are different when grouped by the two class labels (`+` and `-`).\n",
        "\n",
        "For the 6 continuous features, how are they different when split between the two class labels? Choose two features to run t-tests (again split by class label) - specifically, select one feature that is *extremely* different between the classes, and another feature that is notably less different (though perhaps still \"statistically significantly\" different). You may have to explore more than two features to do this.\n",
        "\n",
        "For the categorical features, explore by creating \"cross tabs\" between them and the class label, and apply the Chi-squared test to them. There are 9 categorical features - as with the t-test, try to find one where the Chi-squared test returns an extreme result (rejecting the null that the data are independent), and one where it is less extreme.\n",
        "\n",
        "**NOTE** - \"less extreme\" just means smaller test statistic/larger p-value. Even the least extreme differences may be strongly statistically significant.\n",
        "\n",
        "Your *main* goal is the hypothesis tests, so don't spend too much time on the exploration/visualization piece. That is just a means to an end. This is challenging, so manage your time and aim for a baseline of at least running two t-tests and two Chi-squared tests before polishing. And don't forget to answer the questions in part 3, even if your results in this part aren't what you want them to be."
      ]
    },
    {
      "metadata": {
        "id": "_nqcgc0yzm68",
        "colab_type": "code",
        "colab": {}
      },
      "cell_type": "code",
      "source": [
        "# TODO"
      ],
      "execution_count": 0,
      "outputs": []
    },
    {
      "metadata": {
        "id": "ZM8JckA2bgnp",
        "colab_type": "text"
      },
      "cell_type": "markdown",
      "source": [
        "## Part 3 - Analysis and Interpretation\n",
        "\n",
        "Now that you've looked at the data, answer the following questions:\n",
        "\n",
        "- Interpret and explain the two t-tests you ran - what do they tell you about the relationships between the continuous features you selected and the class labels?\n",
        "- Interpret and explain the two Chi-squared tests you ran - what do they tell you about the relationships between the categorical features you selected and the class labels?\n",
        "- What was the most challenging part of this sprint challenge?\n",
        "\n",
        "Answer with text, but feel free to intersperse example code/results or refer to it from earlier."
      ]
    },
    {
      "metadata": {
        "id": "LIozLDNG2Uhu",
        "colab_type": "text"
      },
      "cell_type": "markdown",
      "source": [
        "*Your words here!*"
      ]
    }
  ]
}
