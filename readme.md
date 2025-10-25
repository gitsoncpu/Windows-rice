## ✨ Basic stuff ✨

#### AltSnap https://github.com/RamonUnch/AltSnap ``` fork of AltDrag ```
#### MSEdgeRedirct https://github.com/rcmaehl/MSEdgeRedirect ``` forces windows search to default browser ```

### uBlock elements
```
music.youtube.com##.cast-button.style-scope.ytmusic-cast-button
! YT Homepage and Subscriptions (Grid View) - Hide the Shorts section
youtube.com##[is-shorts]
! YT Menu - Hide the Shorts button
www.youtube.com###guide [title="Shorts"], .ytd-mini-guide-entry-renderer[title="Shorts"]
! YT Search - Hide Shorts
www.youtube.com##ytd-search ytd-video-renderer:has([overlay-style="SHORTS"],[href^="/shorts/"])
! YT Search, Channels, Subscriptions (List View) and Sidebar/Below Player Recommendations - Hide the Shorts sections
www.youtube.com##ytd-reel-shelf-renderer
! YT Channels - Hide the Shorts tab
www.youtube.com##[tab-title="Shorts"]
! YT Subscriptions - Hide Shorts - Grid View
www.youtube.com##ytd-browse[page-subtype="subscriptions"] ytd-grid-video-renderer:has([overlay-style="SHORTS"],[href^="/shorts/"])
! YT Subscriptions - Hide Shorts - List View
www.youtube.com##ytd-browse[page-subtype="subscriptions"] ytd-video-renderer:has([overlay-style="SHORTS"],[href^="/shorts/"])
! YT Subscriptions - New Layout - Hide Shorts
www.youtube.com##ytd-browse[page-subtype="subscriptions"] ytd-rich-item-renderer:has([overlay-style="SHORTS"],[href^="/shorts/"])
! YT Sidebar - Hide Shorts
www.youtube.com###related :is(ytd-compact-video-renderer,yt-lockup-view-model):has([overlay-style="SHORTS"],[href^="/shorts/"])

! YT Mobile - Hide the Shorts Menu button
m.youtube.com##ytm-pivot-bar-item-renderer:has(>.pivot-shorts)
! YT Mobile - Hide the Shorts sections
m.youtube.com##ytm-reel-shelf-renderer
m.youtube.com##ytm-rich-section-renderer:has([d^="M17.77,10.32l-1.2"])
! YT Mobile - Hide Shorts in search results
m.youtube.com##ytm-search ytm-video-with-context-renderer:has([data-style="SHORTS"])
! YT Mobile - Hide the Shorts button on Channels
m.youtube.com##[tab-title="Shorts"]
! YT Home - Hide Mixes
youtube.com##ytd-rich-item-renderer:has([href*="start_radio=1"])
! YT Sidebar - Hide Mixes
youtube.com##ytd-compact-radio-renderer, :is(#related yt-lockup-view-model,ytd-compact-video-renderer):has([href*="&start_radio=1"])
! YT Search- Hide Mixes
youtube.com##ytd-radio-renderer, :is(ytd-search yt-lockup-view-model,ytd-video-renderer[is-search]):has([href*="&start_radio=1"][aria-label])
! YT Player - Hide Mixes in Video End Cards
youtube.com##.ytp-videowall-still[data-is-mix="true"]

! YT Sidebar - Hide "YouTube" (Music) playlists
youtube.com##ytd-compact-playlist-renderer:has([title^="YouTube"])

/annotations_module.js$script,xhr,important,domain=youtube.com```

