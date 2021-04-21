<script>
function onConversationsAPIReady() {
    window.HubSpotConversations.on('contactAssociated', function(payload) {
        window.dataLayer.push({
            'event': 'ga_event',
            'eventCategory': 'hubspot chat',
            'eventAction': 'contact associated',
            'eventLabel': ''
        })
    });
    window.HubSpotConversations.on('conversationStarted', function(payload) {
        window.dataLayer.push({
            'event': 'ga_event',
            'eventCategory': 'hubspot chat',
            'eventAction': 'conversation started',
            'eventLabel': payload.conversation.conversationId
        })
    });
}
if (window.HubSpotConversations) {
    onConversationsAPIReady();
} else {
    window.hsConversationsOnReady = [onConversationsAPIReady];
}
</script>
