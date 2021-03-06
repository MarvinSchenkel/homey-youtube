# YouTube media player

Search YouTube and play found video in media player.  
Play playlists  
Play music directly on Homey _(experimental)_  

### Trigger cards
- YouTube media changed - triggered when search finishes or playlist item changes

### Action cards
- Search YouTube - play predefined video
- Search YouTube (live) - searches dynamic query (i.e. from speech)
- Get YouTube playlist - fethes playlist and triggers media changed trigger
- Stop YouTube playlist - stops playlist

### Speech support

- "watch Adele from YouTube"; triggers "YouTube media changed"
- "play Adele from YouTube"; plays music on Homey

### API support

Other apps can consume YouTube API using this app.

```javascript
Homey.manager('api').get('/app/com.youtube/search?q=hello', function (err, result) {
    Homey.log(result)
})
```

### Screenshots

![Search YouTube action][action-search-image]  
![Search Live YouTube action][action-live-image]  
![Playlist autoplay support][action-playlist-image]  
![YouTube media change trigger][trigger-change-image]  

Works great with [Chromecast app][chromecast-app].  
![Chromecast cast URL][chromecast-image]

### Donate

If you like the app, buy me a beer!  
[![Paypal donate][pp-donate-image]][pp-donate-link]

Bitcoin address <a href="bitcoin:1DFvxFGFyK11Fr8gTJNeh5xnQMSZCbNgRZ" title="Bitcoin address 1DFvxFGFyK11Fr8gTJNeh5xnQMSZCbNgRZ">1DFvxFGFyK11Fr8gTJNeh5xnQMSZCbNgRZ</a>

![Bitcoin donate][btc-donate-image]]

[chromecast-app]: https://apps.athom.com/app/com.google.chromecast
[action-search-image]: https://cloud.githubusercontent.com/assets/10425/13227043/e2c734b2-d994-11e5-9bdc-fb882b87fdec.png
[action-live-image]: https://cloud.githubusercontent.com/assets/10425/13375135/13b2d002-dd98-11e5-88cd-5892e5ec2af3.png
[action-playlist-image]: https://cloud.githubusercontent.com/assets/10425/13375080/c8be93ca-dd96-11e5-9329-746d520171e5.png
[trigger-change-image]: https://cloud.githubusercontent.com/assets/10425/13227089/228d3eca-d995-11e5-9f90-c4000a243581.png
[chromecast-image]: https://cloud.githubusercontent.com/assets/10425/13375121/b08adcfe-dd97-11e5-9fe9-82ff03286441.png
[pp-donate-link]: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=Y63PX8NDJYVZN&lc=SI&item_number=homey%2dyoutube&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted
[pp-donate-image]: https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif
[btc-donate-image]: https://cloud.githubusercontent.com/assets/10425/15555061/4460fdf4-22c7-11e6-8c4f-f7f0f561721b.png