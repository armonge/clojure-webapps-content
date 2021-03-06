# Add Ring Dependency

As we are using the Ring library for our Clojure project we need to add that library as a project dependency.  Just like other build tools (i.e. Maven, Gradle) we include this dependency in our build file, `project.clj`

> ####Note:: Add the Ring library as a dependency to the project configuration

Edit the `project.clj` file and add **[ring "1.7.1"]** to the `:dependencies` section, typically after the Clojure library dependency.

Whilst editing the project configuration file, you can also update the `:description` section and add a meaningful description of the project and change `:license` to your preferred software license.

```clojure
(defproject todo-list "0.1.0-SNAPSHOT"
  :description "A simple webapp using Ring"
  :url "http://example.com/FIXME"

  :license {:name "Creative Commons Attribution Share-Alike 4.0 International"
            :url  "https://creativecommons.org"}

  :dependencies
    [[org.clojure/clojure "1.10.0"]
     [ring                "1.7.1"]])
```

> ####Hint:: Read the [dependencies secion of the Leiningen documentation](https://github.com/technomancy/leiningen/blob/stable/doc/TUTORIAL.md#dependencies) to learn more about adding libraries.

## Looking up Libraries & current versions

  There are a large number of Clojure libraries available via [Clojars.org](https://clojars.org), an online repository similar to Maven Central.

  Use the Clojars.org website to search for the [latest version of Ring](https://clojars.org/search?q=ring).

![](/images/clojure-webdev-clojars-ring.png)

  The dependency notation for Leiningen and Maven is documented for each library.
