# RemoteImageView

This package offers an Image View to display pictures that are downloaded at runtime by specifying an url.

Usage: First create a RemoteImageFetcher while specifying the url (as an URL-Type). Then create the RemoteImageView with a placeholder Image, the RemoteImageFetcher and a context what happens with the image.

```
let imageFetcher = RemoteImageFetcher(url: URL)
RemoteImageView(placeHolder: Image("PLACEHOLDER"), imageFetcher: imageFetcher) {
        $0
            .resizable()
            .scaledToFit()
    }
```
