# NeuraChat GTM Template

This repository contains a Google Tag Manager (GTM) template for embedding the NeuraChat widget on your website.

## Files Overview

- **`template.tpl`** - The main GTM template file containing the tag configuration
- **`metadata.yaml`** - Template metadata for the GTM Community Template Gallery
- **`LICENSE`** - Apache 2.0 license file
- **`README.md`** - This documentation file

## Installation

### Method 1: Import via GTM Community Template Gallery (Recommended)

1. **Access the Template Gallery**
   - Log into your Google Tag Manager account
   - Navigate to **Templates** in the left sidebar
   - Click **Search Gallery**

2. **Find the NeuraChat Template**
   - Search for "NeuraChat" in the template gallery
   - Click on the NeuraChat template to view details

3. **Install the Template**
   - Click **Add to Workspace** button
   - The template will be added to your workspace's template library

4. **Create a New Tag**
   - Go to **Tags** in the left sidebar
   - Click **New** to create a new tag
   - Select **NeuraChat** from the tag type dropdown
   - Configure the tag parameters (see Configuration section below)
   - Set up triggers as needed
   - Save and publish your container

### Method 2: Manual Import (Advanced Users)

1. **Download the Template**
   - Clone or download this repository
   - Locate the `template.tpl` file

2. **Import to GTM**
   - In GTM, go to **Templates** → **Search Gallery**
   - Click **Submit Template** (if you have developer access)
   - Upload the `template.tpl` file
   - Follow the submission process

## Configuration

### Required Parameters

- **Widget ID** - Your NeuraChat widget ID (e.g., `widget-abcdefg1234`)
- **Mode** - Choose between:
  - `bubble` - Floating chat bubble
  - `inline` - Embedded in a specific element

### Optional Parameters

- **Position** (for bubble mode) - Choose `left` or `right` (default: `right`)
- **Element ID** (for inline mode) - The HTML element ID where the widget should be embedded
- **Version** (Advanced) - Specify widget version (default: `latest`)

### Example Configuration

#### Bubble Mode
```
Widget ID: widget-abc123def456
Mode: bubble
Position: right
```

#### Inline Mode
```
Widget ID: widget-abc123def456
Mode: inline
Element ID: chat-container
```

## Usage

### Step 1: Get Your Widget ID
1. Sign up for a NeuraChat account
2. Create a new widget in your NeuraChat dashboard
3. Copy the widget ID provided

### Step 2: Configure the Tag
1. In GTM, create a new tag using the NeuraChat template
2. Enter your widget ID
3. Choose the display mode (bubble or inline)
4. Configure additional options as needed

### Step 3: Set Up Triggers
Common trigger configurations:
- **All Pages** - Widget appears on every page
- **Specific Pages** - Widget appears only on certain pages
- **User Interaction** - Widget appears after user action

### Step 4: Test and Publish
1. Use GTM's Preview mode to test the implementation
2. Verify the widget appears correctly
3. Publish your container when ready

## File Descriptions

### template.tpl
The main template file containing:
- Template metadata and branding
- Parameter definitions
- JavaScript code for widget initialization
- Web permissions configuration
- Test scenarios

### metadata.yaml
Contains template metadata for the GTM Community Template Gallery:
- Template information
- Version details
- Change notes
- Gallery submission data

### LICENSE
Apache 2.0 license file required for Google Tag Manager Community Template Gallery submissions.

## Troubleshooting

### Widget Not Appearing
1. Check that your widget ID is correct
2. Verify the tag is firing (use GTM Preview mode)
3. Check browser console for JavaScript errors
4. Ensure the widget script is loading from the CDN

### Inline Mode Issues
1. Verify the element ID exists on the page
2. Check that the element is present when the tag fires
3. Ensure the element has proper dimensions

### Permission Errors
1. Verify web permissions are properly configured
2. Check that the script URL is accessible
3. Ensure no Content Security Policy (CSP) restrictions

## Support

For issues with the GTM template:
- Check the troubleshooting section above
- Review GTM's debugging tools
- Contact NeuraChat support for widget-specific issues

For template development:
- Refer to [GTM Template Development Documentation](https://developers.google.com/tag-manager/templates)
- Review the [GTM Community Template Gallery Guidelines](https://developers.google.com/tag-manager/gallery)

## License

This template is licensed under the Apache 2.0 License. See the [LICENSE](LICENSE) file for details.
