# aim

> ring http server for cljd

**aim** aims to be a simple, small HTTP server for clojure-dart.

It uses [dart.io.HttpServer](https://api.dart.dev/stable/2.17.1/dart-io/HttpServer-class.html)
converts [dart.io.HttpRequest](https://api.dart.dev/stable/2.17.1/dart-io/HttpRequest-class.html) into ring-requests and
ring-responses into [dart.io.HttpResponse](https://api.dart.dev/stable/2.17.1/dart-io/HttpResponse-class.html)

## Usage

Add to your project

```clojure
br.com.souenzzo/aim {:git/url "https://github.com/souenzzo/aim"
                     :git/sha "70d48c6c08b3cde9619a7c723135c8758c8abfd8"}
```

Require `[aim.main :as aim]` namespace

and use it: `(run-server (fn [ring-request] ... ring-response) {:port 8080})`
