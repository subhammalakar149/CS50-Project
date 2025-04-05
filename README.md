PAGE TRANSLATOR EXTENSION

Video Demo: https://youtu.be/Qo6fmeYWzow

Description:

    In short, the project is on a simple fully functional page translator built using HTML, CSS and JavaScript.

    The features of this project includes:

        - A basic and clean Page Translator and a manifest file.

        - A clean intuitive popup interface.

        - Efficient implementation of Javascript to handle translation request and also right injection of the translation of the page when triggered.

        - It is integrated with translation API to provide effective and accurate translations.

Working of the extension,
    To understand the working of the extension, it is highly suggested to go through the Video Demo URL (https://youtu.be/Qo6fmeYWzow) given above.
    We start by installing the extension from local system (extension > manage extensions > developer mode > load unpacked).
    Once the extension in installed succesfully, without any errors, you can start using it for any webpage.
    Simply, click on Extensios, then click on Page Translator.
    There will be a pop-up to choose language, after that select the language from the drop down list and then click on Translate button to translate the whole page.
    To revert back to original language, click on Back on your browser.

    And that's it.

Why did I build this?
    Any information you want to know is searched on web, and since there are people in my country, education wise backward who can't interprete the language english could
    use the extension to know the information in their native language.
    Yes, there is already page translation available in most web browsers, but i wanted to get my hands to build one to know the working of this feature.
    Also, in future if i build web application, it would come in handy, to make my web application extra user friendly.

Explanation of each files contained in this project :

    background.js
        The JavaScript code is for a Google Chrome extension.It ensures that when the extension is installed or updated, a confirmation message ("Page Translator Extension Installed.") appears in the console. It's useful for debugging or notifying the developer/user that the extension installation process has been successful.

    langs.js
        The JavaScript code in it defines an array called languages that contains a list of objects. Each object represents a language, with two key-value pairs. The array is used for Building a language selection feature in the application (like a dropdown menu for choosing a language). It is also used to display a list of available languages in the extension.

    manifest.json
        The JSON code is the manifest.json file, is essential for a Chrome extension. It provides metadata and specifies the behavior and features of the extension. This manifest is used to create a "Page Translator" Chrome extension, and it outlines the essential components and permissions.

    popup.css
        This CSS code defines the styling for our extension. Breakdown:

        Global Styling (*):
            outline: none;: Removes the default focus outline for all elements.

        body:
            Sets the font to Arial or falls back to sans-serif if Arial isn't available.
            Adds 20px padding around the content.
            Limits the width of the body content to 250px.

        h1:
            Sets the font size of h1 headers to 18px.
            Removes margin around the element (margin: 0;).
            Adds a bottom padding of 10px for spacing.
            Creates a bottom border with a light gray color (#ccc) to visually separate the header.

        label, select, button:
            Adds spacing between elements using margin-top: 10px;.
            Forces these elements to take up the full width of their parent container using width: 100%;.

        select:
            Provides padding for spacing (5px).
            Sets the font size to 14px.
            Changes the mouse cursor to a pointer when hovering over dropdown options.

        button:
            Adds 10px padding for spacing within the button.
            Sets a black background color (#000000) and white text color (#fff).
            Adds a white border and slightly rounds the button corners with a 5px border radius.
            Makes the button interactive with a cursor change to a pointer and a smooth transition effect (transition: all 0.3s ease).
            Changes the background color to dark blue (#00008b) when hovered (button:hover).

    popup.html
        The HTML code represents the structure of a simple Chrome extension popup for our "Page Translator" extension. It creates a user-friendly way to select a language and translate a page with minimal styling and functionality.

    translate.js
        The JavaScript code adds a listener for messages sent to a Chrome extension. It integrates translation functionality into the extension. When the extension receives a message with a target language, it redirects the current tab to Google Translate, translating the webpage into the specified language.

    popup.js
        The JavaScript code is designed to dynamically populate a language dropdown menu and handle the translation functionality in a Chrome extension. This code achieves two key functionalities:
            Language Dropdown Setup:
                Dynamically populates the dropdown menu with languages, ensuring flexibility and ease of updates.
            Translation Trigger:
                Upon clicking the button, the code sends the selected language to the active tab, enabling page translation functionality through the translate.js script.

