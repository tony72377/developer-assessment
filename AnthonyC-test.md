
**Scheduled Live Stream Video Events**

The major challenge I see in designing and developing this new streaming platform is to make sure that 
the video streaming and products purchases integrate with each other seamlessly. 
The user should be able to chat and view/purchase a product without ever moving away from the live stream.
I think the best way to achieve this is to make use of the speed and flexibility offered by the combination of node.js and React.js.

The way I see the layout is the left 2/3rds of the screen being taken up by the stream and the chat the remaining 1/3. 
At the top or bottom of the stream, a shortlist of featured products can be displayed with a button in the top right that will open a modal 
to the right of the stream where the user will be able to scroll or search all of Misen's products. 
The user should then be able to add to the cart and finish their transaction without leaving the stream.
Also, physical products don't have to be the only thing sold. User privileges and special emotes packaged into subscription tiers can also be sold. 
Those subscription tiers can help with user engagement and really make the user feel like they more than just a spectator.
For the live chat, the best-prebuilt option would probably be Twilio. 
Most if not all of their services already have integrations with react and it allows for administrator level privileges to allow moderation of the chat.

For notifying users of a scheduled stream there are several options with the most basic being Mailchimp but FireBase's notification system is more feature-rich 
with the only 'downside' being the integration with the server but it is probably well worth it especially when it comes to how quickly the notifications can be 
sent out. Speaking of the server, I would suggest either Amazon's EC2 or S3 servers. 
They would provide great reliability and scalability as the site grows and attracts more users. 
A CDN like either Cloudflare or Amazon's own Cloudfront should definitely be used as well in order to make sure the video content 
is streamed with low latency and as little buffering as possible and it can also manage certain sitewide optimization tasks.

**Posts About New Products**

I would use Auth0 or another similar service to both authenticate users and authorize posts for different user types/levels.
I would look to make it easy for post authors to add tags to any post in order to make them easily searchable. 
Once the posts are live then notifications should also be sent out just as with the video streams to attract more attention.
For the surveys on the posts, you can either work with a custom form or for ease of use and less development time an integration with SurveyMonkey can be used.
And for the comment section, React has a library called react-comments-section which can help in quickly building out a comment section that can be moderated by 
Misen administrators. As only registered users will be able to see these posts spam shouldn't be much of an issue but just in case an integration with Askimet or 
another anti-spam service can be integrated.

Okay, hope this wasn't too long. I just wanted to say thanks for going through the interview process with me and that you find the perfect fit you're looking for!



