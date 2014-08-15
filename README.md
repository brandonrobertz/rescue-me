# Rescue Me!

![Rescue Me! logo](/path/to/img.jpg)

Rescue Me! is a webapp that makes linking animal shelters with
people looking to adopt simple and painless.

All it requires is a Google Doc with a list of currently
adoptable animals and their information.

Edit one line inside `js/app.js` to point at the spreadsheet, and point your users
at a beautifully filter-able listing!

## Usage

### 0. Fork Rescue Me!

You're already half way there! Forking Rescue Me will automatically set
up your own Rescue Me website under your github account.

### 1. Create your Google Spreadsheet

An example spreadsheet for the (Wags And Licks)[http://wagsandlicks.org/] is
located (here)[https://docs.google.com/spreadsheets/d/1y-kJ2lehFeMEn4avPAzf1b7RfsYTKL19fsznK8qaP_w/edit#gid=0]. It needs the fields

    Name
    Sex
    Age
    Breed
    Size
    Weight
    Energy Level
    Spayed or Neutered
    Child Friendly?
    Description
    Medical Issues
    In Foster Care?
    Intake Date

It's OK to leave out some of the fields, they just won't show up when
a user searches using that field.

Now make the Spreadsheet publicly-accessible.

### 2. Link the Spreadsheet to Rescue Me!

You'll need the Google Spreadsheet Key, which can be found in the URL of the doc:


                                          .-  The key starts here (after the slash)
                                          ||
                                          \/
    https://docs.google.com/spreadsheets/d/1y-kJ2lehFeMEn4avPAzf1b7RfsYTKL19fsznK8qaP_w/edit#gid=0
                                                                                      ^
                                                                                      |
                                                And it ends here (before the slash)  -'


Open `js/app.js` and find the line:

    var URL = "1y-kJ2lehFeMEn4avPAzf1b7RfsYTKL19fsznK8qaP_w";

Replace the key with your Google spreadsheet's key.
