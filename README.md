# Final-Project-cloud
The gundam Website API is a simple API organized around REST.

Core Resources
Agree
This is an object represents how many people vote which character. There are two methods.

GET
This retrieves the total count of how many people have agreed to cats being awesome. This calls AWS Gateway API which then calls the lambda function voteJazz2. The lambda function then accesses the DynamoDb Agree table, and returns the count.

Sample Call

This is a simple GET call, and requires no body.

Sample Response

{
    statusCode: 201,
            body: '',
            headers: {
                'Access-Control-Allow-Origin': '*',
            },
    }
}
POST
This post an agreement to count towards how many people have agreed to cats being awesome. This calls AWS Gateway API which then calls the lambda function AgreeCats. The lambda function then accesses the DynamoDb Agree table, and writes the new agreement to the table.

Sample Call

This POST call requires no body.

Sample Response

{
 statusCode: 201,
            body: '',
            headers: {
                'Access-Control-Allow-Origin': '*',
            },
    }
}
jazzread
GET
This is an object represents how many people vote which character.

Sample Call

This is a simple GET call, and requires no body.

Sample Response

{
 statusCode: 201,
            body: '',
            headers: {
                'Access-Control-Allow-Origin': '*',
            },
    }
    POST
This post an agreement to count towards how many people have agreed to cats being awesome. This calls AWS Gateway API which then calls the lambda function AgreeCats. The lambda function then accesses the DynamoDb Agree table, and writes the new agreement to the table.


