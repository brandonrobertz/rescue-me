# Rescue Me!

![Rescue Me! logo](http://brandonrobertz.github.io/rescue-me/css/images/rescueme.png)

Rescue Me! is a webapp that makes linking animal shelters with people looking to adopt simple and painless. All it requires is a Google Doc with a list of currently adoptable animals and their information.

You can find the running version at: [http://brandonrobertz.github.io/rescue-me/](http://brandonrobertz.github.io/rescue-me/). It currently features dogs from [Wags And Licks Dog Rescue](http://wagsandlicks.wordpress.com/contact-us/).

## Usage

### 0. Fork Rescue Me!

You're already half way there! Forking Rescue Me will automatically set
up your own Rescue Me website under your github account. Your URL will be:

    http://[Your GitHub Username].github.io/rescue-me/

### 1. Create your Google Spreadsheet

An example spreadsheet for the [Wags And Licks Dog Rescue](http://wagsandlicks.org/) is
located [here](https://docs.google.com/spreadsheets/d/1BZFRwle-r0BVwhzWqmSV8QfdmFVdtPRD3sENYftt-JE). It needs the fields:

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
    Adoption Contact

You can make a copy into your own Google Docs account by clicking on `File -> Make a Copy ...`

Once you have your own copy you need to link it in the app (next step).

### 2. Link the Spreadsheet to Rescue Me!

Once you've made whatever changes you need inside your own copy of the Google spreadsheet,
you need to make it accessible publicly. Do that by clicking on `File -> Publish to the Web...`

Choose the settings, I leave mine default "Entire Document" and "Web Page", and then a
link will appear. You need to copy that link. It will look like this:

    https://docs.google.com/spreadsheets/d/1BZFRwle-r0BVwhzWqmSV8QfdmFVdtPRD3sENYftt-JE

Open `js/app.js` and find the line:

    var URL = "https://docs.google.com/spreadsheets/d/1BZFRwle-r0BVwhzWqmSV8QfdmFVdtPRD3sENYftt-JE";

Replace the URL with your Google spreadsheet's public web URL.

## Roadmap

Here are a list of features we want to implement next:

1. Scraping tool for all shelters/rescues in Austin.
2. Secondary sheet for people to add dogs to, for insertion into main list. Sort of like a moderation queue.
