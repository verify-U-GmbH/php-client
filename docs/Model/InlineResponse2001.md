# # InlineResponse2001

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**state** | **string** | OAuth parameter in format &#x60;[CLIENT_REFERENCE_ID]:[SESSION_ID]&#x60; supplied to identification gateway | [optional] 
**rejected** | **bool** | Indicates whether identification has been rejected | [optional] 
**rejection_cause** | **string** | Identification rejection cause | [optional] 
**id_document** | [**\OpenAPI\Client\Model\InlineResponse2001IdDocument**](InlineResponse2001IdDocument.md) |  | [optional] 
**id_document_back** | [**\OpenAPI\Client\Model\InlineResponse2001IdDocumentBack**](InlineResponse2001IdDocumentBack.md) |  | [optional] 
**id_document_secondary** | [**\OpenAPI\Client\Model\InlineResponse2001IdDocumentSecondary**](InlineResponse2001IdDocumentSecondary.md) |  | [optional] 
**primary_id_document_number** | **string** | Number of the primary ID document | [optional] 
**first_name** | **string** | The client&#39;s first name | [optional] 
**last_name** | **string** | The client&#39;s last name | [optional] 
**gender** | **string** | The client&#39;s gender | [optional] 
**date_of_birth** | **string** | The client&#39;s date of birth as represented in MRZ of ID document | [optional] 
**address** | **string** | The client&#39;s address in format provided by ID document | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | Time at which the object was created in notation as defined by RFC 3339, section 5.6 | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)


