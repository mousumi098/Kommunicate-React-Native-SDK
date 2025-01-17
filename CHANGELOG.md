## React Native Kommunicate Chat v1.6.8

- Exposed methods to iOS: updateConversationAssignee and updateConversationInfo
```javascript
    RNKommunicateChat.updateConversationAssignee({
            clientConversationId: "<clientconversationid>",
            conversationAssignee: "<assignee email>"}, (success, error) => {
                console.log("Updated conversation assignee");
            });

    RNKommunicateChat.updateConversationInfo({
            clientConversationId: "<client conversation id>",
            conversationInfo: {
            "test1": "value1",
            "test2": "value2"
            }
        }, (success, error) => {
            console.log("Updated conversation info");
            });
```
- HTML Rich Message Video template - Android
- Fixed showing empty body for rich message having no text - Android
- Fix for attachment sending empty message - Android
- Sync deleted message from dashboard - Android
- Optimized group list API - Android
- Fixed empty notification body - Android
- Added Text to Speech Support for messages. To enable it, add this in AppDelegate didFinishLaunchingWithOptions method: 'Kommunicate.defaultConfiguration.enableTextToSpeechInConversation = true' - iOS