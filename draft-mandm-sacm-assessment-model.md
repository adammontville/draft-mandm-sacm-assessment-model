---
title: SACM Endpoint Assessment Model
abbrev: Collection Model
docname: draft-mandm-sacm-assessment-model-latest
stand_alone: true
ipr: trust200902
area: Security
wg: SACM Working Group
kw: Internet-Draft
cat: std
coding: us-ascii
pi:
  toc: yes
  sortrefs: yes
  symrefs: yes

author:
- ins: A. Montville
  name: Adam W. Montville
  org: Center for Internet Security
  abbrev: CIS
  email: adam.w.montville@gmail.com
  street: 31 Tech Valley Drive
  code: '12061'
  city: East Greenbush
  region: NY
  country: USA
- ins: B. Munyan
  name: Bill Munyan
  org: Center for Internet Security
  abbrev: CIS
  email: bill.munyan.ietf@gmail.com
  street: 31 Tech Valley Drive
  code: '12061'
  city: East Greenbush
  region: NY
  country: USA

normative:


informative:



--- abstract

This memo describes an information model (and associated data model) that can be used to encapsulate detailed endpoint attribute expressions for the purpose of performing collection of actual endpoint attributes in support of assessment.

WORKING GROUP: The source for this draft is maintained in GitHub.  Suggested changes should be submitted as pull requests at https://github.com/adammontville/draft-mandm-sacm-assessment-model.  Instructions are on that page as well.

--- middle


# Introduction

TBD

# Terms and Definitions

TBD

#  IANA Considerations

TBD

#  Security Considerations

TBD

#  Acknowledgements

TBD

#  Change Log

TBD


# Contributors
TBD

--- back

# Initial XML
[Convert the assessment XML to a schema that references the others?]

    <assessment>
      <collection>
        <namespace>
        <type></type>  
        <keys>           
          <key>          
            <name>      
            <datatype>
            <operation>  
            <nil>     
            <value>
          </key>
        </keys>
        <behaviors>     
          <behavior>
            <name>
            <datatype>   
            <value>
          </behavior>
        </behaviors>
        <filters>
          <filter>
            <action></action>
            <filter-keys>
              <filter-key>
                <name>
                <datatype>
                <operation>
                <nil>
                <value>
              </filter-key>
            </filter-keys>
          </filter>
        </filters>
      </collection>
      <system-characteristics>
        <item>
          <namespace></namespace>
          <type></type>
          <status></status>
          <unique-identifier></unique-identifier>
          <fields> <!-- The list of elements in this item -->
            <field> <!-- A single element in this item -->
              <name></name>
              <datatype></datatype>
              <value></value>
              <records> <!-- A "list of rows from the database" -->
                <record> <!-- A "single row" from the database -->
                  <record-name></record-name>
                  <record-fields> <!-- A "list of columns in the row" -->
                    <record-field> <!-- A "single column" in the row -->
                      <record-field-name></record-field-name>
                      <record-field-datatype></record-field-datatype>
                      <record-field-value></record-field-value>
                    </record-field>
                  </record-fields>
                </record>
              </records>
            </field>
          </fields>
        </item>
      </system-characteristics>
      <evaluation>
        <existence-check>
        <item-check>
        <comparison>
          <fields>
           <field>
              <name>
              <datatype>
              <operation>  // Enum, with new value "isNil"
              <value>
            </field>
          </fields>
        </comparison>
      </evaluation>=
    </assessment>

# The Attic

TBD
