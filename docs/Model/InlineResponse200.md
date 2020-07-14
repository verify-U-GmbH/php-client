# # InlineResponse200

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **string** | The client&#39;s address in format provided by ID document | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | Time at which the object was created in notation as defined by RFC 3339, section 5.6 | [optional] 
**date_of_birth** | **string** | The client&#39;s date of birth as represented in MRZ of ID document | [optional] 
**first_name** | **string** | The client&#39;s first name | [optional] 
**gender** | **string** | The client&#39;s gender | [optional] 
**id** | **string** | ID of this ID document | [optional] 
**id_document** | [**\OpenAPI\Client\Model\IdentificationsIdDocument**](IdentificationsIdDocument.md) |  | [optional] 
**id_document_back** | [**\OpenAPI\Client\Model\IdentificationsIdDocumentBack**](IdentificationsIdDocumentBack.md) |  | [optional] 
**id_document_secondary** | [**\OpenAPI\Client\Model\IdentificationsIdDocumentSecondary**](IdentificationsIdDocumentSecondary.md) |  | [optional] 
**last_name** | **string** | The client&#39;s last name | [optional] 
**primary_id_document_number** | **string** | Number of the primary ID document | [optional] 
**rejected** | **bool** | Indicates whether identification has been rejected | [optional] 
**rejection_cause** | **string** | Identification rejection cause | [optional] 
**state** | **string** | OAuth parameter in format &#x60;[CLIENT_REFERENCE_ID]:[SESSION_ID]&#x60; supplied to identification gateway | [optional] 
**status** | **string** | Identification status | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)


