# willda-tv-callback

A single static page used as the Spotify sign-in redirect for Willda TV, a
home dashboard for Fire TV.

Spotify only redirects to HTTPS addresses, while Willda TV runs on the home
network. After you sign in, Spotify sends you here; the page forwards the
one-time sign-in code to the TV's local address (carried in the `state`
parameter) and only to a private network address. It stores nothing and
contains no secrets.
