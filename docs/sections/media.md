# Media Section

A Media section is composed as a two-column box with a media object on one side and related text on the other. The media section  supports a variety of media types. It supports images, videos, icons, audio and animated lottie files, which are selected via the `mediaType` field. By default, the text is located on the left of the media column. The field `reverse`  can be used to reverse the order of the media and text columns.

## Fields
```
component: media
disabled: false
inContainer: true
marginTop: false
marginBottom: true
paddingTop: false
paddingBottom: true
reverse: false
backgroundColor: ""
targetId: ""
text:
  title: Quam Ridiculus Ornare
  header: "h2"
  subTitle: Nulla vitae elit libero, a pharetra augue.
  prose: Etiam porta sem malesuada magna mollis euismod...
hasCtas: true
ctas:
  - url: "https://github.com/wernerglinka/ms-components"
    label: Get the Starter
    isExternal: true
    isButton: true
    buttonStyle: "primary"
    isVideoTrigger: false
    videoId: ""
mediaType: Image
video:
  src: youtube
  id: ""
  tn: ""
  aspectRatio: ""
  caption:
image:
  src: "v1664225756/company-starter/pexels-anamul-rezwan-1145434_w33asu.jpg"
  alt: "Metalsmith Javascript"
  aspectRatio: "66.67"
  caption: "Photo by Anamul Rezwan from Pexels"
lottieData:
  src: ""
  control:
    autoplay: true
    loop: true
icon: ""
audio:
  bgImage: ""
  aspectRatio: ""
  ogg: ""
  mpeg: ""
  caption:
```

## Notes
