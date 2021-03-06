# List Item
Suitable for presenting a summary of an item with associated actions. Most often used within a List component. It was designed to represent an email message on desktop computers and is not currently touch friendly.

## Variants

### Default
<!---
{{> ListItemElem props=ListItemModels.basic }}
--->

### Image
The same as the default variant, with a thumbnail image added.

<!---
{{> ListItemElem props=ListItemModels.image }}
--->

### Document
Showcases a document by providing a thumbnail, title, and some metadata.
<!---
{{> ListItemElem props=ListItemModels.document }}
--->

## States

### Selectable
Apply the `is-selectable` class to make it possible to select the item.
<!---
{{> ListItemElem props=ListItemModels.selectable }}
--->

### Selected
When applied alongside the `is-selectable` class, `is-selected` will mark it as selected.
<!---
{{> ListItemElem props=ListItemModels.selected }}
--->

### Unseen
Use `is-unseen` to indicate that the item has not been seen.
<!---
{{> ListItemElem props=ListItemModels.unseen }}
--->

### Unread
Use `is-unread` to indicate that the item has not been read.
<!---
{{> ListItemElem props=ListItemModels.unread }}
--->

## Using this component
1. Confirm that you have references to Fabric's CSS and JavaScript on your page, as well as jQuery:
    ```
    <head>
        <link rel="stylesheet" href="fabric.min.css">
        <link rel="stylesheet" href="fabric.components.min.css">
        <script src="jquery-2.2.1.min.js"></script>
        <script src="jquery.fabric.min.js"></script>
    </head>
    ```
2. Copy the HTML from one of the samples above into your page.
3. Add the following `<script>` tag to your page, below the references to jQuery and Fabric's JS, to instantiate all Dialog components on the page:
    ```
    <script>
        $(document).ready(function() {
            if ($.fn.ListItem) {
                $('.ms-ListItem').ListItem();
            }
        });
    </script>
    ```
4. Verify that the component is working the same as in the sample above.
5. Replace the sample HTML content (such as the content of `.ms-ListItem-primaryText`) with your content.

## Dependencies
This component has no dependencies on other components, although it is most often used within a List component.

## Accessibility
More details will be added here.

<!---
{{> ListItemJS }}
--->
