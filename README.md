# v
Real time communication  system
{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "collapsed_sections": []
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "source": [
        "# Basic Python"
      ],
      "metadata": {
        "id": "McSxJAwcOdZ1"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 1. Split this string"
      ],
      "metadata": {
        "id": "CU48hgo4Owz5"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "s = \"Hi there Sam!\".\n",
        "\n",
        "\n"
      ],
      "metadata": {
        "id": "s07c7JK7Oqt-"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "string =\"Hi there Sam!\"\n",
        "print(string.split())\n"
      ],
      "metadata": {
        "id": "6mGVa3SQYLkb",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "f0daeaf3-3926-4c23-c538-f30fc3b59625"
      },
      "execution_count": 1,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "['Hi', 'there', 'Sam!']\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 2. Use .format() to print the following string. \n",
        "\n",
        "### Output should be: The diameter of Earth is 12742 kilometers."
      ],
      "metadata": {
        "id": "GH1QBn8HP375"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "planet = \"Earth\"\n",
        "diameter = 12742"
      ],
      "metadata": {
        "id": "_ZHoml3kPqic"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "planet = \"Earth\"\n",
        "diameter = \"12742\"\n",
        "print(\"The diameter of{} is {} kilometer.\".format(planet,diameter ))"
      ],
      "metadata": {
        "id": "HyRyJv6CYPb4",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "3b820a63-dd4a-462e-e4eb-cabf5823e4d8"
      },
      "execution_count": 2,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "The diameter ofEarth is 12742 kilometer.\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 3. In this nest dictionary grab the word \"hello\""
      ],
      "metadata": {
        "id": "KE74ZEwkRExZ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "d = {'k1':[1,2,3,{'tricky':['oh','man','inception',{'target':[1,2,3,'hello']}]}]}"
      ],
      "metadata": {
        "id": "fcVwbCc1QrQI"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "d = {'k1':[1,2,3,{'trichy':['oh','man','inception',{'target':[1,2,3,'hello']}]}]}\n",
        "print(d['k1'][3][\"trichy\"][3]\n",
        "      ['target'][3])"
      ],
      "metadata": {
        "id": "MvbkMZpXYRaw",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "cb7dd149-c320-4855-8451-6acf5c793125"
      },
      "execution_count": 3,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "hello\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Numpy"
      ],
      "metadata": {
        "id": "bw0vVp-9ddjv"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import numpy as np"
      ],
      "metadata": {
        "id": "LLiE_TYrhA1O"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 4.1 Create an array of 10 zeros? \n",
        "## 4.2 Create an array of 10 fives?"
      ],
      "metadata": {
        "id": "wOg8hinbgx30"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import numpy as np\n",
        "array = np.zeros(10)\n",
        "print(\"An array of 10 zeros:\")\n",
        "print(array)"
      ],
      "metadata": {
        "id": "NHrirmgCYXvU",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "520ac886-cf6b-46be-f499-54f6796c9940"
      },
      "execution_count": 6,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "An array of 10 zeros:\n",
            "[0. 0. 0. 0. 0. 0. 0. 0. 0. 0.]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "import numpy as np\n",
        "array = np.ones(10)*5\n",
        "print(\"An array of 10 fives:\" )\n",
        "print(array)\n",
        "  "
      ],
      "metadata": {
        "id": "e4005lsTYXxx",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "c370b63e-0b1c-4d76-fb7b-abc3a3433f37"
      },
      "execution_count": 7,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "An array of 10 fives:\n",
            "[5. 5. 5. 5. 5. 5. 5. 5. 5. 5.]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 5. Create an array of all the even integers from 20 to 35"
      ],
      "metadata": {
        "id": "gZHHDUBvrMX4"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import numpy as np\n",
        "array = np.arange(20,35,2)\n",
        "print(\"Array of all the even integers from 20 to 35\")\n",
        "print(array)"
      ],
      "metadata": {
        "id": "oAI2tbU2Yag-",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "96f11a4e-284a-4110-aaee-bbb5a15f5cc8"
      },
      "execution_count": 8,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Array of all the even integers from 20 to 35\n",
            "[20 22 24 26 28 30 32 34]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 6. Create a 3x3 matrix with values ranging from 0 to 8"
      ],
      "metadata": {
        "id": "NaOM308NsRpZ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import numpy as np\n",
        "matrix = np.arange(0,9).reshape(3,3)\n",
        "print(matrix)"
      ],
      "metadata": {
        "id": "tOlEVH7BYceE",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "2e215719-05f9-430e-a39a-7da4be2c4091"
      },
      "execution_count": 10,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[[0 1 2]\n",
            " [3 4 5]\n",
            " [6 7 8]]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 7. Concatenate a and b \n",
        "## a = np.array([1, 2, 3]), b = np.array([4, 5, 6])"
      ],
      "metadata": {
        "id": "hQ0dnhAQuU_p"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import numpy as np \n",
        "a = np.array([1, 2, 3])\n",
        "b = np.array([4, 5, 6])\n",
        "c = np.concatenate((a,b),axis=0)\n",
        "print(c)"
      ],
      "metadata": {
        "id": "rAPSw97aYfE0",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "fb98c161-13c5-44d1-9aab-6298b49d8a81"
      },
      "execution_count": 11,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1 2 3 4 5 6]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Pandas"
      ],
      "metadata": {
        "id": "dlPEY9DRwZga"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 8. Create a dataframe with 3 rows and 2 columns"
      ],
      "metadata": {
        "id": "ijoYW51zwr87"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import pandas as pd\n"
      ],
      "metadata": {
        "id": "T5OxJRZ8uvR7"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "import pandas as pd\n",
        "df = pd.DataFrame(columns=['name','dept'], index=['1','2'])\n",
        "df.loc['1'] = ['abi','IT']\n",
        "df.loc['2'] = ['ram','CSE']\n",
        "df.loc['3'] = ['preethi','ECE']\n",
        "print(df)"
      ],
      "metadata": {
        "id": "xNpI_XXoYhs0",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "05bb43d4-b755-47a5-f62a-7ae9c00f51d7"
      },
      "execution_count": 12,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "      name dept\n",
            "1      abi   IT\n",
            "2      ram  CSE\n",
            "3  preethi  ECE\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 9. Generate the series of dates from 1st Jan, 2023 to 10th Feb, 2023"
      ],
      "metadata": {
        "id": "UXSmdNclyJQD"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "import pandas as pd\n",
        "dates = pd.date_range('01-01-2023','02-10-2023')\n",
        "s = pd.Series(dates)\n",
        "print(s)"
      ],
      "metadata": {
        "id": "dgyC0JhVYl4F",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "201a3c80-2f4a-4438-8cf6-ee5b72fd635e"
      },
      "execution_count": 14,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0    2023-01-01\n",
            "1    2023-01-02\n",
            "2    2023-01-03\n",
            "3    2023-01-04\n",
            "4    2023-01-05\n",
            "5    2023-01-06\n",
            "6    2023-01-07\n",
            "7    2023-01-08\n",
            "8    2023-01-09\n",
            "9    2023-01-10\n",
            "10   2023-01-11\n",
            "11   2023-01-12\n",
            "12   2023-01-13\n",
            "13   2023-01-14\n",
            "14   2023-01-15\n",
            "15   2023-01-16\n",
            "16   2023-01-17\n",
            "17   2023-01-18\n",
            "18   2023-01-19\n",
            "19   2023-01-20\n",
            "20   2023-01-21\n",
            "21   2023-01-22\n",
            "22   2023-01-23\n",
            "23   2023-01-24\n",
            "24   2023-01-25\n",
            "25   2023-01-26\n",
            "26   2023-01-27\n",
            "27   2023-01-28\n",
            "28   2023-01-29\n",
            "29   2023-01-30\n",
            "30   2023-01-31\n",
            "31   2023-02-01\n",
            "32   2023-02-02\n",
            "33   2023-02-03\n",
            "34   2023-02-04\n",
            "35   2023-02-05\n",
            "36   2023-02-06\n",
            "37   2023-02-07\n",
            "38   2023-02-08\n",
            "39   2023-02-09\n",
            "40   2023-02-10\n",
            "dtype: datetime64[ns]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "## 10. Create 2D list to DataFrame\n",
        "\n",
        "lists = [[1, 'aaa', 22],\n",
        "         [2, 'bbb', 25],\n",
        "         [3, 'ccc', 24]]"
      ],
      "metadata": {
        "id": "ZizSetD-y5az"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "lists = [[1, 'aaa', 22], [2, 'bbb', 25], [3, 'ccc', 24]]"
      ],
      "metadata": {
        "id": "_XMC8aEt0llB"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "import pandas as pd\n",
        "data = [[1,'aaa',22],[2,'bbb',25],[3,'ccc',24]]\n",
        "df = pd.DataFrame(data)\n",
        "print(df)"
      ],
      "metadata": {
        "id": "knH76sDKYsVX",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "f1eae41e-1820-4bdf-d43a-6167a580fe39"
      },
      "execution_count": 15,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "   0    1   2\n",
            "0  1  aaa  22\n",
            "1  2  bbb  25\n",
            "2  3  ccc  24\n"
          ]
        }
      ]
    }
  ]
}
