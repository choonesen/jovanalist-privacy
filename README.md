# looplockers-privacy

The privacy policy for the [LoopLockers](https://apps.apple.com/) iOS app,
served by GitHub Pages at **<https://choonesen.github.io/looplockers-privacy/>**.

That URL is what App Store Connect points at, so it has to stay reachable. Apple
requires a privacy policy URL for every app, including apps that collect nothing
— which this one doesn't.

## Don't edit `index.html` here

It is a **copy**. The policy is written in the app's own repository, at
`store/privacy-policy.html`, so that the words Apple links to and the words the
app itself shows can be checked against each other. This repo exists only
because Pages needs a public one and the app's repo is private.

Editing the copy makes the two disagree, and the one that is wrong is the one
nobody looks at. It has happened: the live page spent a release missing the
paragraph explaining that a reminder shows an item's own words on the lock
screen.

## Updating it

From the app repository:

```sh
./scripts/publish-privacy.sh "What changed"
```

That copies the file, pushes it here, and waits until Pages is actually serving
the new version before it reports success.
