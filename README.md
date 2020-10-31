# backend-test

## Description
The main functionalities of this software are:
1 – Registering a vessel. The vessel data input is its code, which can’t be repeated (return the HTTP code appropriate and an
error message if the user tries to register a existing code). For instance, a valid input of a vessel is: “code”: “MV102”.
2 – Registering a new equipment in a vessel. The data inputs of each equipment are name, code, location and status. Each
equipment is associated to a given vessel and has a unique code, which can’t be repeated (return the HTTP code appropriate
and an error message if the user tries to register a existing code). For each new equipment registered, the equipment status is
automatically active. For instance, a valid input of a new equipment related to a vessel “MV102” is:

{

"name": "compressor",
"code": "5310B9D7",
"location": "Brazil"

}

3 – Setting an equipment’s status to inactive. The input data should be one or a list of equipment code.
4 – Returning all active equipment of a vessel
