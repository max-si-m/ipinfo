# Ipinfodb

This's simple gem for (http://ipinfodb.com/)[http://ipinfodb.com/]

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'ipinfo'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install ipinfo

## Usage
Use your api key for site, you can get it (here)[http://ipinfodb.com/account.php]
```
ip_info = IpInfo::API.new('<api_key>')   
```
And use `#lookup` for geting information about *ip*:
```
ip_info.lookup('209.85.227.104', type: 'city', timezone: true)
```
or *domain*:
```
ip_info.lookup('devbattles.com', type: 'city', timezone: true)
```


## Contributing

1. Fork it ( https://github.com/[my-github-username]/ipinfo/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
