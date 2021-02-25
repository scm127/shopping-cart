# shopping-cart
This Readme.md is adopted from my Rock Paper Scissors Exercise Readme.  It explains how to clone the repository, and allows the user to add grocery store products by their product identifier and prints their receipt which includes all items purchased as well as the total amount spent. 

# Prerequisites:
```sh
Anaconda 3.7+
Python 3.7+
Pip
```

# Installing the Repository
Fork this remote repository under your own control, then "clone" or download your remote copy onto your local computer.

Navigate to the repository from the command line (subsequent commands assume you are running them from the local repository's root directory). If you saved the repository to your desktop use the following code or else you will have to adjust the code to wherever the repository is saved:
```sh
cd ~/Desktop/shopping-cart
```
# Create and activate virtual enviorment
Use Anaconda to create and activate a new virtual environment, perhaps called "my-game-env":

```sh
conda create -n shopping-env python=3.8
conda activate shopping-env
```

From inside the virtual environment, install package dependencies. The requirmemnts.txt file has the Dotenv package which is needed to load enviorment variables as well as the sendgrid package which is needed to send emails:
```sh
pip install -r requirements.txt
```
# Setup local variables
In the root directory of your local repository, create a new file called ".env", and update the contents of the ".env" file to specify the tax rate in the area. The user can also add the variables SENDGRID_API_KEY and SENDER_ADDRESS if they want an email of their receipt. To get the SENDGRIP_API_KEY they must make an account on SendGrid. 

```sh
tax_rate=.0875
SENDGRID_API_KEY=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
SENDER_ADDRESS=scm127@georgetown.edu
```

# Run the Shopping Cart Python Script and follow the instructions to input product identifiers for the desired products:
```sh
python shopping_cart.py
```
Note that if anything something is inputed that is not a product idetifier, the user will be asked to please input a valid product identifier.  

