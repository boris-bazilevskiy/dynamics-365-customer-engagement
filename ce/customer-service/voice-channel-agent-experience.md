---
title: "Use agent dashboard and call controls in the voice channel | MicrosoftDocs"
description: "Use this article to understand how the agent can use the agent dashboard, use call controls, and also make and receive customer calls in Omnichannel for Customer Service."
ms.date: 11/18/2022
ms.service: dynamics-365-customerservice
ms.topic: article
author: gandhamm
ms.author: mgandham
manager: shujoshi
---

# Use agent dashboard and call controls in the voice channel

[!INCLUDE[cc-use-with-omnichannel](../includes/cc-use-with-omnichannel.md)]

The voice channel in Omnichannel for Customer Service is integrated directly with Dynamics 365 by way of the agent dashboard. The dashboard offers you as an agent a consolidated view of the calling interface, the customer summary, case history, and timeline. This helps you provide quick, effective, and proactive solutions to customer issues. The agent experience in the voice channel is similar to the chat and other channels, which reduces agent training time and costs.

## Make and receive customer calls

You can call a customer by using the phone dialer on the customer summary page or the **Launch dialer** button on the menu. More information: [Call a customer](voice-channel-call-customer.md)

When a customer calls your business, the incoming call is received by an intelligent bot. The bot gathers basic information about the customer issue and then transfers the call to you for further action. You'll receive a notification about the incoming call on your agent desktop so you can accept it. The following section describes the call controls and other features you can use during your conversation.

## Call controls

The conversation panel in the agent dashboard includes the following call controls that you can use when you call or answer phone calls from customers.

> [!div class="mx-imgBorder"]
> ![Screenshot of call controls.](./media/voice-channel-call-controls.png)

- **Mute**: Mute your microphone so your voice isn't audible to the customer.
- **Hold**: Put the customer on hold; the customer will hear the hold music. You can keep only one caller on hold at a time.
- **Consult**: Select this option to consult with a participant. You can consult with or bring another agent or supervisor into the call. You can have a *public* consultation, where the customer is actively involved in the conversation. Or you can have a *private* consultation, where you can put the customer on hold before you talk to your peers or supervisor.
> [!NOTE]   
> When you initiate a consult, you are the primary agent and the new participant has a consult role. Select **Transfer** next to the participant to transfer the call to the consulting agent or supervisor. Once the call is transferred, you are the consulting agent and can leave the call without ending the call. The consulting agent becomes the primary agent. If the primary agent leaves the call, the call will end for the customer.

- **Transfer**: Select this option is to transfer the call to an agent, queue, a Teams user, or an external phone number. Once you transfer the call, the agent to whom the call is transferred is the primary agent and you will no longer be on the call. 
    During a transfer to the queue, the customer is automatically put on hold. When you transfer a call to another agent, your number is displayed on the caller ID. The transcription and recording of transferred calls will continue if the administrator has enabled the [option](voice-channel-configure-transcripts.md#enable-call-recording-and-transcription-for-voice). You can disable recording from the dashboard. See: [Transfer and consult scenarios](voice-channel-transfer-consult.md)
- **End**: End the call.
- **Show number pad**: Open the number pad so you can dial an extension number, when required. If you must use the dial pad to send a response while navigating an IVR , select the dial pad icon next to the external participant in the participant list.
- **Mark number as spam**: [Report the incoming call as spam](#report-a-phone-number-as-spam). If you happened to accidentally mark a number as spam, you can select the **Unmark as spam** option.
- **Device settings**: Configure your microphone and speaker settings.
- **Take notes**: Make note of important information or specific details from your conversation with the customer. It's in addition to the call recording and transcription that happen during the conversation.
- **Pause transcription**: If you don't want to capture some details of the conversation—such as bank details, billing, or payment information—you can temporarily pause the transcription and resume it later.
- **Knowledge Articles**: Get a list of knowledge base articles pertaining to the conversation that you can use to resolve the customer issue.
- **Link to conversation**: You can link another conversation, case, or knowledge article to the conversation.
- **Transcription**: When the transcription and recording service is enabled by your administrator, the conversation between you and the customer is automatically transcribed in real time, which means that you as an agent don't need to take notes during the call. This feature also helps your supervisor or agent (in a call transfer) to see the call history.
- **Sentiment analysis**: The transcript also powers *live* sentiment analysis. This means that you or your supervisor can instantly view and gauge the customer's mood and feeling via the sentiment icons.

## Access and listen to voicemails (preview)

> [!NOTE]
> The voicemail feature is in preview. [!INCLUDE[cc-preview-features-definition](../includes/cc-preview-features-definition.md)]

You can access the voicemails recorded by customers on your direct inward dial number or through work items that have been routed to you in one of the following ways:

- On the **Customer Service Agent Dashboard**, in **My Open Activities**, select the vertical ellipses, and then select **Other Activities** > **Voicemail (Preview)**.
- On the **Omnichannel Agent Dashboard**, in **Open work items**, select the vertical ellipses for your number, and then select **Assign to me**.
- If inbox is configured for you, you can view the assigned and unassigned voicemails. Go to your inbox, and select **Assigned voicemails**, and then select the voicemail that you want to hear. If you access an unassigned voicemail and then close it, you won't be able to access it again.

## Report a phone number as spam

You can report a phone number as a spam call while you're on the call by using the call controls on the conversation panel. A notification is then sent to your administrator for review and further action.

To report a phone number as spam, select the ellipsis to open more actions, and then select **Mark number as spam**.

You can add notes to help your administrator review and block numbers. After you mark a number as spam, it goes into the pending review tab on the **Blocked numbers** page.

## How to avoid call disconnection

Ensure the following behaviors to avoid call drops:

- Don't refresh your browser when you're in an active call. When you select refresh, even if you select cancel on the confirm refresh dialog, the page is unloaded, and the call is disconnected.
- Don't select browser bookmark icons on the Customer Service workspace or Omnichannel for Customer Service app browser tab when you're in the middle of an ongoing call.
- Don't open other apps that will need access to the microphone.
- Don't open the Customer Service workspace or Omnichannel for Customer Service app in more than one tab in the browser.
- Always select the **End** button and then close the session. Don't close the session directly to end call.

### See also

[Overview of the voice channel](voice-channel.md)  
[Enable voice consult with Microsoft Teams users](voice-consult-microsoft-teams-user.md)  
[Make and receive your first call](voice-channel-first-call.md)  
[Call a customer](voice-channel-call-customer.md)  

[!INCLUDE[footer-include](../includes/footer-banner.md)]
