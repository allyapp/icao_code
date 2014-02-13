# ICAOCode

Automate finding ICAO codes, using OpenFlights data.

http://openflights.org/data.html

## Installation

After cloning repository:

    $ bundle
    $ bundle exec rake install

## Usage

Search ICAO codes by given airline name.

CLI: 

    $ icao_code find lufthansa
    Lufthansa: DLH
    Lufthansa Cargo: GEC
    Lufthansa CityLine: CLH
    Lufthansa Systems: 
    Lufthansa Technik: LHT
    
Plain Ruby:

```ruby
result = result = ICAOCode.lookup("lufthansa") // => {"Lufthansa"=>"DLH", "Lufthansa Cargo"=>"GEC", "Lufthansa CityLine"=>"CLH", "Lufthansa Systems"=>"", "Lufthansa Technik"=>"LHT"}
```
