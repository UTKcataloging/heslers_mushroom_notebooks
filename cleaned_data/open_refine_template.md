# Open Refine Template for L.R. Hesler’s Mushroom Research Notebooks (TRACE Migration)

## Template

#### Prefix

```
<?xml version="1.0" encoding="UTF-8"?>
<modsCollection xmlns="http://www.loc.gov/mods/v3" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http://www.w3.org/1999/xlink" xsi:schemaLocation="http://www.loc.gov/mods/v3 http://www.loc.gov/standards/mods/v3/mods-3-5.xsd">
```
####Body

```
<mods>
<identifier type="filename">{{cells['filename'].value}}</identifier>
<titleInfo supplied="yes"><title>{{cells["title"].value}}</title></titleInfo> 
<abstract>{{cells['abstract'].value}}</abstract>
{{if(isBlank(cells['date_text'].value), '', '<originInfo><dateCreated>' + cells['date_text'].value + '</dateCreated><dateCreated encoding="edtf" keyDate="yes" point="start" qualifier="inferred">' + cells['date_edtf'].value + '</dateCreated><dateCreated encoding="edtf" keyDate="yes" point="end" qualifier="inferred">' + cells['date_edtf_end'].value + '</dateCreated></originInfo>')}}
{{if(isBlank(cells['dateIssued'].value), '', '<originInfo><dateIssued>' + cells['dateIssued'].value + '</dateIssued><dateIssued keyDate="yes" encoding="edtf">' + cells['date_edtf'].value + '</dateIssued></originInfo>')}}
<physicalDescription><form authority="aat" valueURI="{{cells['form_URI'].value}}">{{cells['form'].value}}</form><digitalOrigin>reformatted digital</digitalOrigin></physicalDescription>
{{if(isBlank(cells['subject'].value), '', '<subject authority="lcsh"><topic>' + cells['subject'].value + '</topic></subject>')}}
{{if(isBlank(cells['subject2'].value), '', '<subject authority="lcsh"><topic>' + cells['subject2'].value + '</topic></subject>')}}
{{if(isBlank(cells['subject3'].value), '', '<subject authority="lcsh"><topic>' + cells['subject3'].value + '</topic></subject>')}}
{{if(isBlank(cells['subject_uncontrolled'].value), '', '<subject><topic>' + cells['subject_uncontrolled'].value + '</topic></subject>')}}
{{if(isBlank(cells['subject_name'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name_URI'].value + '><namePart>' + cells['subject_name'].value + '</namePart></name></subject>')}}
<language><languageTerm authority="iso639-2b" type="text">English</languageTerm></language>
<typeOfResource>text</typeOfResource>
{{if(isBlank(cells['type2'].value), '', '<typeOfResource>' + cells['type2'].value + '</typeOfResource>')}}
<relatedItem displayLabel="Collection" type="host"><titleInfo><title>L.R. Hesler Botanical Research Notebooks</title></titleInfo><identifier>MS.3751</identifier></relatedItem>
<relatedItem displayLabel="Project" type="host"><titleInfo><title>{{cells['digital_collection'].value}}</title></titleInfo></relatedItem>
<location><physicalLocation authority="naf" valueURI="http://id.loc.gov/authorities/names/no2014027633">University of Tennessee, Knoxville. Special Collections</physicalLocation></location>
<recordInfo><languageOfCataloging><languageTerm authority="iso639-2b" type="text">English</languageTerm></languageOfCataloging><recordOrigin>Created and edited in general conformance to MODS Guidelines (Version 3.5).</recordOrigin><recordContentSource valueURI="http://id.loc.gov/authorities/names/n87808088">University of Tennessee, Knoxville. Libraries</recordContentSource></recordInfo>
<accessCondition type="use and reproduction" xlink:href="http://rightsstatements.org/vocab/InC/1.0/">In Copyright</accessCondition>
</mods>
```

#### Suffix

```
</modsCollection>
```