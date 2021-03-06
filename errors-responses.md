# HTTP Status Codes

The HeiaHeia API attempts to return appropriate [HTTP status codes](http://en.wikipedia.org/wiki/List_of_HTTP_status_codes) for every request.

<table>

<thead>

<tr>

<th width="15%">Code</th>

<th width="25%">Text</th>

<th>Description</th>

</tr>

</thead>

<tbody>

<tr>

<td>200</td>

<td>OK</td>

<td>Success!</td>

</tr>

<tr>

<td>304</td>

<td>Not Modified</td>

<td>There was no new data to return.</td>

</tr>

<tr>

<td>400</td>

<td>Bad Request</td>

<td>The request was invalid or cannot be otherwise served. An accompanying error message will explain why.</td>

</tr>

<tr>

<td>401</td>

<td>Unauthorized</td>

<td>Authentication credentials were missing or incorrect.</td>

</tr>

<tr>

<td>403</td>

<td>Forbidden</td>

<td>The request is understood, but it has been refused or access is not allowed. An accompanying error message will explain why.</td>

</tr>

<tr>

<td>404</td>

<td>Not Found</td>

<td>The URI requested is invalid or the resource requested, such as a user, does not exists.</td>

</tr>

<tr>

<td>500</td>

<td>Internal Server Error</td>

<td>Something is broken.</td>

</tr>

<tr>

<td>502</td>

<td>Bad Gateway</td>

<td>HeiaHeia is down or being upgraded.</td>

</tr>

</tbody>

</table>

# Error Messages

All error objects have message and code properties so that your client can tell what the problem is. Error code to let you know what is wrong with the request.

<div class="snippet">

    [
      { "code": 34, "message": "Sorry, that page does not exist" }
    ]

</div>

Error messages contain machine-parseable codes. While the text for an error message may change, the codes will stay the same.These are the possible validation error codes:

<table>

<thead>

<tr>

<th width="15%">Code</th>

<th width="25%">Text</th>

<th>Description</th>

</tr>

</thead>

<tbody>

<tr>

<td>34</td>

<td>Sorry, that page does not exist</td>

<td>Corresponds with an HTTP 404 - the specified resource was not found.</td>

</tr>

</tbody>

</table>
