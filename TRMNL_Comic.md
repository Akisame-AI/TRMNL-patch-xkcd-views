# How to Set Up the Daily Comic from xkcd

<kbd>![daily-comic-rankings-plugin](https://github.com/SnarfulSolutionsGroup/TRMNL-Plugins/blob/main/Daily_Comic.png)</kbd>

There are 2 ways to add plugins to TRMNL. Automatic and Manual. 
## Automatic
Log in to your TRMNL dashboard.  
On the left-hand menu, click on the 'Go to Plugins' button.  
Find the 'Private Plugin' Plugin to create a Private Plugin.  
Click 'import new' to import the plugin zip file found in this repository.  
Click 'Save' to save the plugin. 

## Manual
## Step 1: Create a New Private Plugin
Log in to your TRMNL dashboard.
On the left-hand menu, click on the 'Go to Plugins' button.
Find the 'Private Plugin' Plugin to create a Private Plugin.
Click 'Add new' to create a new Private Plugin.

## Step 2: Set up the Polling Strategy
Name your plugin (e.g., "Daily Comic") then scroll down to the Strategy section.
Choose the Polling strategy from the Strategy dropdown menu.
In the Polling URL field, enter this URL:

```
https://xkcd.com/info.0.json
```
Click Save. Once it is saved, the 'Edit Markup' button is now available.

## Step 3: Add the HTML Markup
Click the 'Edit Markup' button.

Copy and paste the following code into the Markup box. This code will display a daily comic supplied from xkcd.
```
<div class="view comic-view bg-white">
  <div class="layout layout--col gap--space-between">
    <div class="columns">
      <div class="column">
        <div class="content content">
          <!-- Centered Comic Image -->
          <img src="{{ img }}" alt="{{ title }}" style="display: block; margin: 0 auto; max-width: 90vw; max-height: 87vh; border-radius: 5px;">
        </div>
      </div>
    </div>
  </div>
  <div class="title_bar">
    <!-- Left-Aligned Title Bar Content -->
    <img class="image" src="https://xkcd.com/s/0b7742.png" alt="xkcd Logo" />
    <span class="title">xkcd Comic</span>
    <span class="instance"><strong>{{ title }}</strong></span>
  </div>
</div>

```
Other views require other markup files (included in the repository)

## Step 4: Save and Activate the Plugin
Once you have entered the markup, click Save to store the plugin.
Navigate to the Playlists tab in your TRMNL dashboard.
Drag and drop your new Daily Comic plugin to the top of your playlist if not automatically added.

## Step 5: View the Daily Comic on Your Device
Once refreshed, your TRMNL device will display the Daily Comic.
