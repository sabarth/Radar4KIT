Appendix 
++++++++

Basic metadata scheme at RADAR .XML
===================================

.. code-block:: xml
    <xs:schema targetNamespace="http://radar-service.eu/schemas/descriptive/radar/v09/radar-dataset" elementFormDefault="qualified">
<xs:import namespace="http://radar-service.eu/schemas/descriptive/radar/v09/radar-elements" schemaLocation="RadarElements.xsd"/>
<xs:element name="radarDataset">
<xs:complexType>
<xs:sequence>
<xs:element ref="re:identifier"/>
<xs:element ref="re:alternateIdentifiers" minOccurs="0"/>
<xs:element ref="re:relatedIdentifiers" minOccurs="0"/>
<xs:element ref="re:creators"/>
<xs:element ref="re:contributors" minOccurs="0"/>
<xs:element ref="re:title"/>
<xs:element ref="re:additionalTitles" minOccurs="0"/>
<xs:element ref="re:descriptions" minOccurs="0"/>
<xs:element ref="re:keywords" minOccurs="0"/>
<xs:element ref="re:publishers"/>
<xs:element ref="re:productionYear"/>
<xs:element ref="re:publicationYear" minOccurs="0"/>
<xs:element ref="re:language" minOccurs="0"/>
<xs:element ref="re:subjectAreas"/>
<xs:element ref="re:resource"/>
<xs:element ref="re:geoLocations" minOccurs="0"/>
<xs:element ref="re:dataSources" minOccurs="0"/>
<xs:element ref="re:software" minOccurs="0"/>
<xs:element ref="re:processing" minOccurs="0"/>
<xs:element ref="re:rights"/>
<xs:element ref="re:rightsHolders"/>
<xs:element ref="re:relatedInformations" minOccurs="0"/>
<xs:element ref="re:fundingReferences" minOccurs="0"/>
</xs:sequence>
</xs:complexType>
</xs:element>
</xs:schema>



Example Radar4KIT .XML
======================

.. code-block:: xml

    <?xml version="1.0" encoding="UTF-8" standalone="yes"?>
    <ns2:radarDataset xmlns="http://radar-service.eu/schemas/descriptive/radar/v09/radar-elements" xmlns:ns2="http://radar-service.eu/schemas/descriptive/radar/v09/radar-dataset">
    <identifier identifierType="DOI">10.1111/gcb.13004</identifier>
    <alternateIdentifiers>
        <alternateIdentifier alternateIdentifierType="Type of alternative identifier, e.g. internal identifier">Identifier other than RADARs persistent identifier e.g. institute specific identifier used to identify the data</alternateIdentifier>
    </alternateIdentifiers>
    <relatedIdentifiers>
        <relatedIdentifier relatedIdentifierType="bibcode" relationType="IsCitedBy">Identifier of complementary material related to this resource e.g. a scientific article</relatedIdentifier>
    </relatedIdentifiers>
    <creators>
        <creator>
            <creatorName>The person(s) responsible for the content of the research data e.g. the data producer. Format: Surname, First (given) name or the name of the institution. </creatorName>
            <givenName>GivenName</givenName>
            <familyName>FamilyName</familyName>
            <nameIdentifier schemeURI="http://orcid.org/" nameIdentifierScheme="ORCID">2220-0021-5000-0004</nameIdentifier>
            <creatorAffiliation>Affiliation (only for people)</creatorAffiliation>
        </creator>
    </creators>
    <contributors>
        <contributor contributorType="ContactPerson">
          <contributorName>People or Institutions involved in the creation of the resource. Format: Surname, First (given) name or the name of the institution. </contributorName>
          <givenName>GivenName</givenName>
          <familyName>FamilyName</familyName>
          <nameIdentifier schemeURI="http://orcid.org/" nameIdentifierScheme="ORCID">2220-0021-5000-0004</nameIdentifier>
          <contributorAffiliation>Affiliation (only for people)</contributorAffiliation>
        </contributor>
    </contributors>
    <title>Dataset example</title>
    <additionalTitles>
        <additionalTitle additionalTitleType="TranslatedTitle">Alternative or additional information to the main title of the resource e.g. the translated title</additionalTitle>
    </additionalTitles>
    <descriptions>
        <description descriptionType="Abstract">A description containing additional information about the resource. English is strongly recommended as the primary language. </description>
    </descriptions>
    <keywords>
        <keyword>Include keyword(s) that describe the subject focus of the resource. Format: Comma-separated list of keywords. </keyword>
    </keywords>
    <publishers>
        <publisher>Include the person(s) or organisation responsible for archiving or publishing the resource. </publisher>
    </publishers>
    <productionYear>2015-2016</productionYear>
    <language>eng</language>
    <subjectAreas>
        <subjectArea>
            <controlledSubjectAreaName>Agriculture</controlledSubjectAreaName>
        </subjectArea>
    </subjectAreas>
    <resource resourceType="Dataset">General information on the content of the resource. </resource>
    <geoLocations>
        <geoLocation>
            <geoLocationCountry>GERMANY</geoLocationCountry>
            <geoLocationRegion>Spatial region, country or place where the data was collected or which the data refers to. </geoLocationRegion>
            <geoLocationBox>
                <southWestPoint>
                    <latitude>29.612</latitude>
                    <longitude>54.668</longitude>
                </southWestPoint>
                <northEastPoint>
                    <latitude>38.29</latitude>
                    <longitude>80.728</longitude>
                </northEastPoint>
            </geoLocationBox>
        </geoLocation>
        <geoLocation>
            <geoLocationCountry>GERMANY</geoLocationCountry>
            <geoLocationRegion>Place/region e.g. Europe</geoLocationRegion>
            <geoLocationPoint>
                <latitude>50.1136</latitude>
                <longitude>9.25087</longitude>
            </geoLocationPoint>
        </geoLocation>
    </geoLocations>
    <dataSources>
        <dataSource dataSourceDetail="Other">Specify the origin of the data contained in the resource</dataSource>
    </dataSources>
    <software>
        <softwareType type="Other">
            <softwareName softwareVersion="Software version">Software name</softwareName>
            <alternativeSoftwareName alternativeSoftwareVersion="Software version">Software name</alternativeSoftwareName>
        </softwareType>
    </software>
    <processing>
        <dataProcessing>Specify the instructions used for processing the data in the digital resource (e.g. statistics). </dataProcessing>
    </processing>
    <rights>
        <controlledRights>CC BY-NC 4.0 Attribution-NonCommercial</controlledRights>
    </rights>
    <rightsHolders>
        <rightsHolder>Specify the person(s) or institution(s) who own or manage the intellectual property rights of the dataset. Format: Surname, First (given) name or the name of the institution. </rightsHolder>
    </rightsHolders>
    <relatedInformations>
        <relatedInformation>Please specify, for example, the related information on the sample used to produce the digital data in the resource. </relatedInformation>
    </relatedInformations>
    
    <fundingReferences>
      <fundingReference>
        <funderName>DFG</funderName>
        <funderIdentifier type="CrossRefFunder">http://dx.doi.org/10.13039/501100001659</funderIdentifier>
        <awardNumber>BE 1042/7-1</awardNumber>
        <awardURI>http://gepris.dfg.de/gepris/projekt/237143194</awardURI>
        <awardTitle>RADAR Research Data Repositorium</awardTitle>
      </fundingReference>
      <fundingReference>
        <funderName>Test</funderName>
        <funderIdentifier type="ISNI">033000012150090X</funderIdentifier>
        <awardNumber>BE 1042/7-1</awardNumber>
        <awardURI>http://gepris.dfg.de/gepris/projekt/237143194</awardURI>
        <awardTitle>RADAR Research Data Repositorium</awardTitle>
      </fundingReference>
    </fundingReferences>
    </ns2:radarDataset>
