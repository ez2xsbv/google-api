---
title: Adding a GitHub webhook
menu:
  webhooks-main:
    weight: 3
---
Registering Webhooks for Github, to make release packages.

## Get the webhook URL for GitHub

1. Go to the **Code** tab of your app's page and in the **INCOMING WEBHOOKS** menu, click **SETUP MANUALLY**.
2. Select **GitHub** from the dropdown menu.

   ![Screenshot](https://github.com/bitrise-io/devcenter/blob/master/img/github-webhook-1.png)
3. Copy the webhook URL for the selected service.

## Set up webhook on GitHub

1. Navigate to your GitHub repository and select **Settings**.

   ![Screenshot](https://github.com/bitrise-io/devcenter/blob/master/img/webhooks/github-webhook-2.png)
2. Select **Add webhook** under **Webhooks**.

   ![Screenshot](https://github.com/bitrise-io/devcenter/blob/master/img/webhooks/github-webhook-3.png)
3. Paste the GitHub Webhook URL https://packagist.org/api/github?username=**Your_username** to the **Payload URL**
4. Set **Content-Type** to **application/json**
5. Paste the API token to the **Secret** input.

   ![Screenshot](https://github.com/bitrise-io/devcenter/blob/master/img/webhooks/github-webhook-4.png)
4. And on the same page, select **Let me select individual events**.

   ![Screenshot](https://github.com/bitrise-io/devcenter/blob/master/img/webhooks/github-webhook-5.png)
5. Select **Releases**. After you are ready press the **Add webhook** button and you are ready to roll!