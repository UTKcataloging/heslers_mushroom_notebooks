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
<identifier type="filename">{{cells['identifier'].value}}</identifier>
<titleInfo supplied="yes"><title>{{cells["title"].value}}</title></titleInfo> 
<abstract>{{cells['abstract'].value}}</abstract>
<name authority="naf" valueURI="{{cells['author_URI'].value}}"><namePart>{{cells['author'].value}}</namePart><role><roleTerm authority="marcrelator" valueURI="http://id.loc.gov/vocabulary/relators/cre">Creator</roleTerm></role></name>
{{if(isBlank(cells['date_text'].value), '', '<originInfo><dateCreated>' + cells['date_text'].value + '</dateCreated><dateCreated encoding="edtf" keyDate="yes" point="start" qualifier="inferred">' + cells['date_edtf'].value + '</dateCreated><dateCreated encoding="edtf" keyDate="yes" point="end" qualifier="inferred">' + cells['date_edtf_end'].value + '</dateCreated></originInfo>')}}
{{if(isBlank(cells['dateIssued'].value), '', '<originInfo><dateIssued>' + cells['dateIssued'].value + '</dateIssued><dateIssued keyDate="yes" encoding="edtf">' + cells['dateIssued_edtf'].value + '</dateIssued></originInfo>')}}
<physicalDescription><form authority="aat" valueURI="{{cells['form_URI'].value}}">{{cells['form'].value}}</form><digitalOrigin>reformatted digital</digitalOrigin></physicalDescription>
{{if(isBlank(cells['subject'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject_URI'].value + '"><topic>' + cells['subject'].value + '</topic></subject>')}}
{{if(isBlank(cells['subject2'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject2_URI'].value + '"><topic>' + cells['subject2'].value + '</topic></subject>')}}
{{if(isBlank(cells['subject3'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject3_URI'].value + '"><topic>' + cells['subject3'].value + '</topic></subject>')}}
{{if(isBlank(cells['subject4'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject4_URI'].value + '"><topic>' + cells['subject4'].value + '</topic></subject>')}}
{{if(isBlank(cells['subject_uncontrolled'].value), '', '<subject><topic>' + cells['subject_uncontrolled'].value + '</topic></subject>')}}
{{if(isBlank(cells['subject_name'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name_URI'].value + '"><namePart>' + cells['subject_name'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name2'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name2_URI'].value + '"><namePart>' + cells['subject_name2'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name3'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name3_URI'].value + '"><namePart>' + cells['subject_name3'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name4'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name4_URI'].value + '"><namePart>' + cells['subject_name4'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name5'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name5_URI'].value + '"><namePart>' + cells['subject_name5'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name6'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name6_URI'].value + '"><namePart>' + cells['subject_name6'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name7'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name7_URI'].value + '"><namePart>' + cells['subject_name7'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name8'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name8_URI'].value + '"><namePart>' + cells['subject_name8'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name10'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name10_URI'].value + '"><namePart>' + cells['subject_name10'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name11'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name11_URI'].value + '"><namePart>' + cells['subject_name11'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name12'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name12_URI'].value + '"><namePart>' + cells['subject_name12'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name13'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name13_URI'].value + '"><namePart>' + cells['subject_name13'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name14'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name14_URI'].value + '"><namePart>' + cells['subject_name14'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name15'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name15_URI'].value + '"><namePart>' + cells['subject_name15'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name16'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name16_URI'].value + '"><namePart>' + cells['subject_name16'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name17'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name17_URI'].value + '"><namePart>' + cells['subject_name17'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name18'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name18_URI'].value + '"><namePart>' + cells['subject_name18'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name19'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name19_URI'].value + '"><namePart>' + cells['subject_name19'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name20'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name20_URI'].value + '"><namePart>' + cells['subject_name20'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name21'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name21_URI'].value + '"><namePart>' + cells['subject_name21'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name22'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name22_URI'].value + '"><namePart>' + cells['subject_name22'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name23'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name23_URI'].value + '"><namePart>' + cells['subject_name23'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name24'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name24_URI'].value + '"><namePart>' + cells['subject_name24'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name25'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name25_URI'].value + '"><namePart>' + cells['subject_name25'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name26'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name26_URI'].value + '"><namePart>' + cells['subject_name26'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name27'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name27_URI'].value + '"><namePart>' + cells['subject_name27'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name28'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name28_URI'].value + '"><namePart>' + cells['subject_name28'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name29'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name29_URI'].value + '"><namePart>' + cells['subject_name29'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name30'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name30_URI'].value + '"><namePart>' + cells['subject_name30'].value + '</namePart></name></subject>')}}
{{if(isBlank(cells['subject_name31'].value), '', '<subject><name authority="naf" valueURI="' + cells['subject_name31_URI'].value + '"><namePart>' + cells['subject_name31'].value + '</namePart></name></subject>')}}
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