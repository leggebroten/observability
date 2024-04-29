# Observability
A simple repo to demonstrated how to wired up basic observability in a Phoenix app.

We'll start with a basic Phoenix app and show how the basic metrics can be visualized 
with Grafana by having Prometheus scrape the `/metrics` endpoint. 

Then we'll add a custom metric and show how to add a custom span to the metrics. 

Finally, we'll show how to use Telemetry to trace a request through the system.

## Install Elixir, Phoenix, and generate a basic phoenix app.

Install Elixir and phoenix
https://hexdocs.pm/phoenix/installation.html



Generate a basic phoenix app.  Called `observability`
https://hexdocs.pm/phoenix/up_and_running.html

https://cri.dev/posts/2020-05-10-Elixir-trick:-start-an-Observer-window-with-mix/

To give us something to work with, extend it with basic Accounts and Users
https://hexdocs.pm/phoenix/Mix.Tasks.Phx.Gen.Json.html

`mix phx.gen.json Accounts User users name:string age:integer`
`mix ecto.migrate`


## Get basic /metrics working
https://hexdocs.pm/prom_ex/readme.html
* Add[prom_ex.ex](lib%2Fobservability%2Fprom_ex.ex) Ecto metrics.
https://hexdocs.pm/prom_ex/readme.html#setting-up-promex
* Install Prometheus and Grafana.
* Add Phoenix metrics.

## Add a custom metric
* One basic custom metric.

## Add Telemetry tracing
## Add custom span with raw Telemetry
## Context propagation to custom span from controller call
## Replace custom span with @decorate 
## Use Ctor and Protocol to @decorate implementation
## Create new app to show cross-app context propagation


 ## Notes
https://cri.dev/posts/2020-05-10-Elixir-trick:-start-an-Observer-window-with-mix/
https://hexdocs.pm/elixir/debugging.html
http://localhost:4000/dev/dashboard/applications?limit=50&search=&sort_by=name&sort_dir=asc
