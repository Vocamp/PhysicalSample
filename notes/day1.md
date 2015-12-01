Notes for Physical Sample WG - day 1

Steve - There are 4-5 broad areas to start dicussing:
# Sampling/sub-sampling process 
we want to navigate from any parts including transformed parts back to where they came from
A sub-sample isDerivedFrom PhysicalSample

# Parts explosion which is related to the sub-samplling process

# Identify registration which binds the identity to the sample object via some identifier scheme that can be dereferenced
to get the phusical object as well as information about the physical sample telling what the "object means".
# Sample properties

But there is also the issue of the object called collection (not the collection process).

Sampling/sub-sampling process Notes
* Initial idea leveages Prov-O
Physical sample  involves SamplingProcess  redfs:subClassOf PhysicalProcess

Alternative  SampleProcess produces Specimen 
Specimen relatedTerm PhysicalSample
SamplingProcess operates on SamplingFeature. 
SamplingFeature samplesFrom FeatureOfInterest 
 PhysicalSample isA PortionOfMatter but is FeatureofInterest also PortionOfMatter?  Meaning it is composed of something.
 
 A difference might be that the PhysSample is an objct but the Feauture of interest may not be an object.
 When you sample the ocean do you sample water? 

Is the initial sampling process which takes place at some naturtal site with location different than sub-sampling process on the Sample which has a curation/analysis place/organization location?

We think that we can handle some of the issues involved in sub-sample and intentions using Prov-O

<b>Sample Properties Notes </b> (Gary)
Some Sample models (e.g. ODM2) give then attributes like Medium
Sample Medium   The medium in which the sample was collected [e.g. water (Surface Water such as a stream, river, lake, pond,
reservoir, ocean ), air, sediment, etc.
CUAHSI Community Observations Data Model Working Design Specifications Document

Are MaterialType and Medium the same thing (?)
The attribute materialClass:GenericName shall provide a basic classification of the material type of the specimen. 
EXAMPLE Soil, water, rock, aqueous, liquid, tissue, vegetation, food.

Sample Type  & Specimen Type
the attribute specimenType:GenericName shall describe the basic form of the specimen. 

EXAMPLE Polished section; core; pulp; solution.

Some identify sample types as Sample, Field Duplicate, Field Blank, or Reference, generally based on field sample form designation. 
NOAA https://dwhdiver.orr.noaa.gov/field-definitions-and-codes
Samples have identifiers but other attributes (size, weight, color...) that get observed.
geolink:hasIdentifierValue "10.1575/1912/4137" ;
