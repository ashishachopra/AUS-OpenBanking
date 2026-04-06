# Australian Open Banking Data Database
The API specifications for these endpoints can be found [here](https://consumerdatastandardsaustralia.github.io/standards/#future-dated-obligations).

## Getting Started ##
To access any product reference data you need to send a HTTP request with the required parameters to the appropraite banking API URL. The two available Banking APIs are [Get Products](https://consumerdatastandardsaustralia.github.io/standards/#get-products) and [Get Product Detail](https://consumerdatastandardsaustralia.github.io/standards/#get-product-detail).

The easiest way to get started is the Swagger UI [page](https://generator.swagger.io/?url=https://raw.githubusercontent.com/LukePrior/Australian-Open-Banking-Data-Database/main/examples/CDS-Products.yaml) which has all the endpoints imported and the required fields documented.

**Get Products**
This API returns a list of products currently offered by the financial institution to the market.
`https://data.holder.com.au/cds-au/v1/banking/products`

run the following example from CMD.
`curl -X GET https://api.anz/cds-au/v1/banking/products -H "x-v: 3"`

**Get Product Detail**
This API returns detailed information on a single product offered by the financial institutions.
`https://data.holder.com.au/cds-au/v1/banking/products/{productId}`

run the following example from CMD.
`curl -X GET https://api.anz/cds-au/v1/banking/products/5eb62ffc-51f0-6ac0-2abf-d81b260ee260 -H "x-v: 3"`

## Examples
- the [Swagger UI](https://generator.swagger.io/?url=https://raw.githubusercontent.com/LukePrior/Australian-Open-Banking-Data-Database/main/examples/CDS-Products.yaml) to easily test the APIs for any bank.
