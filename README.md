# Lightning Universal Lookup Component
## Powerful lookup component for your developments

Boost the development of your custom components with a new powerful lookup component. It looks like a standard one, pretty easy to customize and works everywhere – even in Salesforce1.

It look like standard field and could be used with Standard and Custom Objects.
<p align="center">
  <img width="90%" src="http://www.synebo.io/servlet/servlet.FileDownload?retURL=%2Fapex%2Fsitearticle%3FpostId%3DLightning_Universal_Lookup_Component&file=00PA000000tK3fGMAS" alt="lookupField">
</p>

***

### Installation

<a href="https://githubsfdeploy.herokuapp.com">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/deploy.png">
</a>

Optionally, you can install it as <a href="https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0Y000002BYze">unmanaged package</a>.
Also available as <a href="https://appexchange.salesforce.com/listingDetail?listingId=a0N3A00000ErH8PUAV">managed package on AppExhange</a>.

***

<p align="center">
  <img width="90%" src="https://image.ibb.co/fT921a/Aura_7.jpg" alt="lookupField">
</p>


```html
<aura:attribute name="selectedId" type="String"/>

<l_lookup:Lookup objectType = "Account" 
                 label = "Customer"
                 selectedRecordId = "{! v.selectedId }"
                 readOnly = "false"
                 showFiveRecent = "false"
                 width="400px">
</l_lookup:Lookup>

```

***

### How to use it

Custom Lookup component field has 6 attributes.

#### Main attributes:	
  * __objectType__ - API name of Salesforce Object. Could be Standard or Custom. 
  * __selectedRecordId__ - variable that will contain Id of selected record.

#### Optional attributes:
  * __label__ - label. Default is label from Object.
  * __width__ - width of field. Default is ‘100%’.
  * __readOnly__ - is field editavle. Default is false.
  * __showFiveRecent__ - feature from standard lookup field, showed 5 recently viewed records. Default is true.


  <p align="center">
    <img width="550" src="https://image.ibb.co/fW4q2Q/ezgif_com_video_to_gif_1.gif" alt="showLastViewed">
  </p>
