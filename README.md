# CometChat React Custom Attachment Integration Guide

## Before

![Chat UI Screenshot](https://www.cometchat.com/docs/assets/images/message_composer_default_attachment_options_web_screens-c569f237c006c80562e098b92692e7a4.png)  
*Alt text: Screenshot of a working CometChat-powered React app with default attachments and active chat visible*

## After
![Chat UI Screenshot](https://www.cometchat.com/docs/assets/images/message_composer_custom_attachment_options_web_screens-104035717491a170e498d72a5a5591a2.png)
*Alt text: Screenshot of a working CometChat-powered React app with custom attachments and active chat visible*

---

## Introduction

This guide helps you add **custom attachment options** (like file upload, location sharing, etc.) to the **CometChat Message Composer** using the React UI Kit.

> Prerequisite: You must have CometChat initialized in your app. If not, refer to the [CometChat Initialization Docs](https://www.cometchat.com/docs/ui-kit/react/react-conversation)

---

## Step 1: Refer to CometChat Initialization Docs

Before integrating custom features, ensure CometChat is properly initialized using your:

- `APP_ID`
- `REGION`
- `AUTH_KEY`

Refer to the [CometChat Initialization Guide](https://github.com/HADES248/CometChatReact-UI-Kit/edit/master/README.md) for more details.

---

## Step 2: Check React UI Kit Documentation

Navigate to the official [CometChat React UI Kit documentation](https://www.cometchat.com/docs/ui-kit/react/message-composer).

In the **Message Composer** section, locate the `AttachmentOptions` prop. This prop accepts a function that allows you to render one or more custom attachment buttons within the composer.

---

## Step 3: Create a Custom Attachment Function

In the file where you render the message composer, define a function that returns your custom attachment actions (e.g., icons for file upload, location sharing).

Each action should have a title, ID, icon, and a handler for what to do when clicked — like opening a file picker or sending a custom message with GPS coordinates.

---

## Step 4: Pass Custom Function to the Composer

Pass the function you created to the `attachmentOptions` prop of the `CometChatMessageComposer` component. This enables the custom buttons in the composer UI.

---

## Final Result

Your message composer now includes additional custom buttons that allow users to:

- Upload and send files
- Trigger any other custom interaction

- [Custom Attachment Code](https://github.com/HADES248/CometChat-CustomAttachment/blob/master/src/App.tsx)

This improves user experience and allows for tailored messaging flows.

---

## Next Steps

- Add Custom Icons or preview popups before sending content
- Customize how custom messages appear in the conversation list and thread view

---
