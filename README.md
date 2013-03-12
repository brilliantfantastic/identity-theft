identity-theft
==============
***

## DESCRIPTION

A test harness for the Stripe API. Provides a stubbed framework for requests and responses for the Stripe API.

## EXAMPLES

```ruby
Inception.define do
  get :customers do
    request:
      id { Faker::Lorem.characters(10) }
    response:
      object "customer"
      created "34567829"
      email "johnny_appleseed@example.com"
  end
end
```
