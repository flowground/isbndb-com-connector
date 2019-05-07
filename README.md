# ![LOGO](logo.png) ISBNdb **flow**ground Connector

## Description

A generated **flow**ground connector for the ISBNdb API (version 1.0.1).

Generated from: https://api.apis.guru/v2/specs/isbndb.com/1.0.1/swagger.json<br/>
Generated at: 2019-05-07T17:42:29+03:00

## API Description

Definition of ISBNdb.com API

## Authorization

Supported authorization schemes:
- API Key
## Actions

### Gets author details

> Returns the name and a list of books by the author.

*Tags:* `Author`

#### Input Parameters
* `name` - _required_ - The name of an author in the Author's database

### Search authors

> This returns a list of authors whos name matches the given query

*Tags:* `Author`

#### Input Parameters
* `pageSize` - _optional_ - How many items should be returned per page, maximum of 1,000
* `query` - _required_ - A string to search for in the Author's database
* `page` - _optional_ - The number of page to retrieve, please note the API will not return more than 10,000 results no matter how you paginate them

### Gets book details

> Returns the book details

*Tags:* `Book`

#### Input Parameters
* `isbn` - _required_ - an ISBN 10 or ISBN 13 in the Books database

### Search books

> This returns a list of books that match the query

*Tags:* `Book`

#### Input Parameters
* `query` - _required_ - A string to search for in the Book's database
* `page` - _optional_ - The number of page to retrieve, please note the API will not return more than 10,000 results no matter how you paginate them
* `author` - _optional_ - Filters the query results by author
* `pageSize` - _optional_ - How many items should be returned per page, maximum of 1,000

### Gets publisher details

> Returns details and a list of books by the publisher.

*Tags:* `Publisher`

#### Input Parameters
* `name` - _required_ - The name of a publisher in the Publisher's database

### Search publishers

> This returns a list of publishers that match the given query

*Tags:* `Publisher`

#### Input Parameters
* `pageSize` - _optional_ - How many items should be returned per page, maximum of 1,000
* `query` - _required_ - A string to search for in the Publisher's database
* `page` - _optional_ - The number of page to retrieve, please note the API will not return more than 10,000 results no matter how you paginate them

### Search all ISBNDB databases

> Uses a free query string compatible with ElasticSearch 6 to search in any of the ISBNDB's databases

*Tags:* `Search`

#### Input Parameters
* `q` - _optional_ - A query string compatible with ElasticSearch 6

### Gets status on the ISBNDB Database

> Returns a status object about the ISBNDB database.

*Tags:* `Stats`

### Gets subject details

> Returns details and a list of books with subject.

*Tags:* `Subject`

#### Input Parameters
* `name` - _required_ - A subject in the Subject's database

### Search subjects

> This returns a list of subjects that match the given query

*Tags:* `Subject`

#### Input Parameters
* `pageSize` - _optional_ - How many items should be returned per page, maximum of 1,000
* `query` - _required_ - A string to search for in the Subject's database
* `page` - _optional_ - The number of page to retrieve, please note the API will not return more than 10,000 results no matter how you paginate them

## License

**flow**ground :- Telekom iPaaS / isbndb-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
