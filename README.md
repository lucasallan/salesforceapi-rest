# Salesforceapi::Rest

TODO: Write a gem description

## Installation

Add this line to your application's Gemfile:

    gem 'salesforceapi-rest'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install salesforceapi-rest

## Usage

    @sf = SalesforceApi::Rest:Client(refresh_token, metadata_url, client_id, client_secret)
    
To create a sobject:
    
    @sf.create(:lead, {:Company => "Company Name", :LastName => "Allan", :Email => "lucas@email.com"})

To get resources information

    @sf.resources
  
To get resources describe

    @sf.describe(:lead)
    
Creating custom fields

    @sf.add_custom_field({:fullName => "Lead.MyCustomField__c", :label => "My Custom Field", :type => "Text"})

  ## License

  ###(The MIT License)

  Copyright (c) 2012 Lucas Allan Amorim (www.lucasallan.com)

  Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ‘Software’), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

  The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

  THE SOFTWARE IS PROVIDED ‘AS IS’, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
