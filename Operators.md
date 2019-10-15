# How to submit?

Once done, make a `zip` of your project folder in a clean state and send it to
`hiring@gettgo.com`.

# Operators

Consider the following set of services and related components under active development:

1. An API server which provides insurance package information.
    * PostgreSQL as database.
    * Connects via static IP address to several third parties.
2. An authentication and order processing API server.
    * Consumes 1)
    * PostgreSQL as a database.
    * Redis as cache.
    * Contains payment data.
3. A node.js web interface written in React.
    * Consumes 2)
    * Stateless

Please write a set of single-cluster kubernetes manifests file to deploy all of the above.
The manifests must include:

1. Scalable deployments (manual).
2. Proper load balancing and ingresses.

BONUS points for:

1. Having proper security isolation.
2. Autoscale.
3. Support multi-cloud deployments.
4. Monitoring system.

