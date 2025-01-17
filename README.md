# Detections

This repo serves as a home for detection content developed by the [delivr.to](https://delivr.to) team.

All rules present in this repo have corresponding payloads (linked in references and shown below) that can be used to test detection content.

The repo currently holds the following types of detections:

- [Sublime Rules](#sublime-rules)
- [Yara Rules](#yara-rules)


## Sublime Rules

Below is the list of rules for Sublime Security, organised into [General](sublime-rules/general/) and [Threat Intel](sublime-rules/threatintel/) specific folders.

You can also integrate delivr.to directly with Sublime as mentioned [here](https://blog.delivr.to/introducing-delivrto-7a8840ff5ed5) and documented [here](https://docs.delivr.to/docs/integrations/sublime_integration.html).

![](assets/delivrto-sublime-integration-results.png)

| Rule Name                                            | Type       | Payload 	| 
|------------------------------------------------------|------------|----------	| 
| [Attachment: HTML file without HTML element (Unsolicited)](sublime-rules/general/attachment_html_file_without_html_elements.yml) 	               | General    |   [![](assets/delivrto.png)]()        | 
| [Attachment: SVG file with Script Tags (Unsolicited)](sublime-rules/general/attachment_svg_with_script_element.yml) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=3dce858d-7be3-412e-85d9-84f3b9845275)        | 
| [Attachment: HTML file with eval function and long byte string (Unsolicited)](sublime-rules/general/attachment_html_eval_byte_string.yml) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=2e5e3a7b-457d-4bd9-8cbe-77d3f403b74c)        | 
| [Attachment: HTML File Containing Recipient Email Address (Unsolicited)](sublime-rules/general/attachment_html_file_with_recipient_email.yml) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=648f544d-a2b0-4968-884e-a5d1a72f51fb)        | 
| [Attachment: Extended HTML File Format (Unsolicited)](sublime-rules/general/attachment_xhtml.yml ) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=44381a80-9269-4974-9d16-a62318ec39f3)        | 
| [Attachment: Microsoft Script Encoding Content](sublime-rules/general/attachment_microsoft_script_encoding_content.yml ) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=e8dce489-d33e-46b5-9e9f-cf2713abd213)        | 
| [Link: Zipped OneNote file](sublime-rules/general/link_zipped_onenote.yml) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=cee09f6e-9cac-4fc9-a033-c69254e6396c)        | 
| [Link: OneNote file](sublime-rules/general/link_onenote.yml) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=ea1b0f0e-fe2b-4ec9-8ba6-56cedf98066e)        | 
| [Link: Brand Impersonation Phishing Site](sublime-rules/general/link_brand_impersonation_phishing_site.yml) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=14bacd0a-a160-4343-80ef-fa7998a32d2d)        | 
| [Attachment: Remote Template Injection](sublime-rules/general/attachment_remote_template_injection.yml) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=ef187d5d-3188-483e-b3b5-9ab5e0e032f7)        | 
| [Attachment: HTML Smuggling with msSaveOrOpenBlob](sublime-rules/general/attachment_mssaveoropenblob.yml) 	               | General    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=be91a311-a023-4221-96da-6f5b717fdc54)        | 
| [Attachment: OneNote file with Suspicious Strings](sublime-rules/threatintel/attachment_onenote_suspicious_strings.yml) 	               | Threat Intel    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=56188625-d386-489e-bf50-604d89675c2a)        | 
| [Link: Zipped OneNote file with Document Download Lure (QakBot)](sublime-rules/threatintel/link_qakbot_zipped_onenote_doc_download_lure.yml) 	               | Threat Intel    |  [![](assets/delivrto.png)](https://delivr.to/payloads?id=cee09f6e-9cac-4fc9-a033-c69254e6396c)         | 
| [Attachment: OneNote containing HTA with VBScript and JavaScript content (QakBot)](sublime-rules/threatintel/attachment_qakbot_onenote_with_hta_containing_javascript_vbscript.yml) 	               | Threat Intel    |     [![](assets/delivrto.png)](https://delivr.to/payloads?id=56188625-d386-489e-bf50-604d89675c2a)      |
| [Attachment: WSF File With Certificate Content (QakBot)](sublime-rules/threatintel/attachment_wsf_cert_file.yml) 	               | Threat Intel    |     [![](assets/delivrto.png)](https://delivr.to/payloads?id=6f7644eb-f31c-4240-8009-48a8db6fb417)      |
| [Attachment: PDF with Document Download Lure](sublime-rules/threatintel/attachment_pdf_with_document_download_lure.yml) 	               | Threat Intel    |     [![](assets/delivrto.png)](https://delivr.to/payloads?id=5d45687f-b2e3-4add-9b2c-71b68eecb169)      |
| [Attachment: PDF with Embedded Google Firebase Storage Link (Bumblebee)](sublime-rules/threatintel/attachment_pdf_with_firebase_link.yml) 	               | Threat Intel    |     [![](assets/delivrto.png)](https://delivr.to/payloads?id=61b6892e-51d9-4840-8446-4a78c80af5cb)      |
| [Attachment: Office Document with Embedded RTF Referencing Remote Resources CVE-2023-36884 (Unsolicited)](sublime-rules/threatintel/attachment_cve_2023_36884.yml) 	               | Threat Intel    |        | 

## Yara Rules

Below is the list of Yara rules in the repo. 

| Rule Name                                            | Type       | Payload 	| 
|------------------------------------------------------|------------|----------	| 
| [SUSP_OneNote_Repeated_FileDataReference_Feb23](yara-rules/onenote_repeated_files.yar)	               | Threat Intel    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=2722d95f-f51d-4ad7-aeb1-60a38e52ae5e)        | 
| [SUSP_OneNote_RTLO_Character_Feb23](yara-rules/onenote_rtlo_filename.yar)	               | Threat Intel    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=44bab49e-21f0-40ef-8851-f9ea70d6b001)        | 
| [SUSP_OneNote_Win_Script_Encoding_Feb23](yara-rules/onenote_windows_script_encoding_file.yar )	               | Threat Intel    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=e8dce489-d33e-46b5-9e9f-cf2713abd213)        | 
| [SUSP_msg_CVE_2023_23397_Mar23](yara-rules/msg_cve_2023_23397.yar )	               | Threat Intel    |   [![](assets/delivrto.png)](https://delivr.to/payloads?id=494a2718-a012-45d5-9fe8-27465b0c1809)        | 
