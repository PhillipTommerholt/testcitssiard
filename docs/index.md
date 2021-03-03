<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

  <meta name="Description" content="">
  <meta name="keywords" content="">

  <!-- Bootstrap CSS -->
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
  <link rel="stylesheet" href="/css/site.css" >

  <title>E-ARK CSIP | E-ARK CSIP</title>
</head>

<body role="document">

  <header id="nav-wrap">
    <div id="nav-cont" class="container">
      <nav id="navbar-main" class="navbar navbar-expand-md" role="navigation">
        <a class="navbar-brand" href="https://dilcis.eu/" title="CSIP main page."><img src="/img/Logo_DILCIS_one_color-v05.png" alt="DILCIS logo" title="DILCIS logo"></a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
           <span class="navbar-toggler-icon"></span>
         </button>
         <div class="collapse navbar-collapse" id="navbarCollapse">
           <ul class="navbar-nav mr-auto">
             
                 
                 <!-- display the top level navigation for items that don’t have a submenu -->
                     
                         <li class="nav-item active">
                     
                     <a class="nav-link" href="/">Specification</a>
                 
                     </li>
             
                 
                 <!-- display the top level navigation for items that don’t have a submenu -->
                     
                         <li class="nav-item">
                     
                     <a class="nav-link" href="/pdf/eark-csip.pdf">PDF</a>
                 
                     </li>
             
                 
                 <!-- display the top level navigation for items that don’t have a submenu -->
                     
                         <li class="nav-item">
                     
                     <a class="nav-link" href="/profile/">Profile</a>
                 
                     </li>
             
                 
                 <!-- display the top level navigation for items that don’t have a submenu -->
                     
                         <li class="nav-item">
                     
                     <a class="nav-link" href="/archive/">Archive</a>
                 
                     </li>
             
                 
                 <!-- display the top level navigation for items that don’t have a submenu -->
                     
                         <li class="nav-item">
                     
                     <a class="nav-link" href="/examples/">Examples</a>
                 
                     </li>
             
                 
                     <li class="dropdown">
                       <a href="/" class="dropdown-toggle" data-toggle="dropdown" data-hover="dropdown">About <span class="caret"></span></a>
                       <ul class="dropdown-menu">
                       
                           
                             <li class="nav-item"><a class="nav-link" href="/release-notes/">Release Notes</a></li>
                           
                       
                           
                             <li class="nav-item"><a class="nav-link" href="https://dilcis.eu/">DILCIS</a></li>
                           
                       
                           
                             <li class="nav-item"><a class="nav-link" href="https://github.com/DILCISBoard/E-ARK-CSIP">On GitHub</a></li>
                           
                       
                           
                             <li class="nav-item"><a class="nav-link" href="https://github.com/DILCISBoard/E-ARK-CSIP/archive/master.zip">Download</a></li>
                           
                       
                       </ul>
                 
                     </li>
             
         </ul>
</div>
       </nav>
    </div>
  </header>

  <div class="container theme-showcase" role="main">
    <h1 id="common-specification-for-information-packages">Common Specification for Information Packages</h1>

<h1 id="preface">Preface</h1>
<h2 id="i-aim-of-the-specification">I. Aim of the Specification</h2>
<p>This document is one of several related specifications which aim to provide a common set of usage descriptions of international standards for packaging digital information for archiving purposes. These specifications are based on common, international standards for transmitting, describing and preserving digital data. They also utilise the Reference Model for an Open Archival Information System (OAIS) which has Information Packages as its foundation. Familiarity with the core functional entities of OAIS is a prerequisite for understanding the specifications.</p>

<p>The specifications are designed to help data creators, software developers and digital archives to tackle the challenge of short-, medium- and long-term data management and reuse in a sustainable, authentic, cost-efficient, manageable and interoperable way.
A visualisation of the current specification network can be seen here:</p>

<p><a name="figi-dip"></a>
<img src="figs/fig_1_dip.svg" alt="OAIS Entities" title="Diagram showing E-ARK specification dependency hierarchy"></p>

<p><strong>Figure I:</strong> Diagram showing E-ARK specification dependency hierarchy.</p>

<h3 id="overview-of-the-e-ark-specifications">Overview of the E-ARK Specifications</h3>

<h4 id="common-specification-for-information-packages-e-ark-csip">Common Specification for Information Packages (E-ARK CSIP)</h4>
<p>This document introduces the concept of a Common Specification for Information Packages (CSIP). The main purposes of CSIP are to:</p>

<ul>
  <li>Establish a common understanding of the requirements which need to be met to achieve interoperability of Information Packages.</li>
  <li>Establish a common base for the development of more specific Information Package definitions and tools within the digital preservation community.</li>
  <li>Propose the details of an XML-based implementation of the requirements using, to the largest possible extent, standards which are widely used in international digital preservation.</li>
</ul>

<p>Ultimately the goal of the Common Specification is to reach a level of interoperability between all Information Packages so that tools implementing the Common Specification can be adopted by institutions without the need for further modifications or adaptations.</p>

<h4 id="specification-for-submission-information-packages-e-ark-sip">Specification for Submission Information Packages (E-ARK SIP)</h4>
<p>The main aims of this specification are to:</p>

<ul>
  <li>Define a general structure for a Submission Information Package format suitable for a wide variety of archival scenarios, such as document and image collections, databases or geospatial data.</li>
  <li>Enhance interoperability between Producers and Archives.</li>
  <li>Recommend best practices regarding the structure, content and metadata of Submission Information Packages.</li>
</ul>

<h4 id="specification-for-archival-information-packages-e-ark-aip">Specification for Archival Information Packages (E-ARK AIP)</h4>
<p>The main aims of this specification are to:</p>

<ul>
  <li>Define a generic structure of the AIP format suitable for a wide variety of data types, such as document and image collections, archival records, databases or geospatial data.</li>
  <li>Recommend a set of metadata related to the structural and the preservation aspects of the AIP as implemented by the reference implementation (earkweb).</li>
  <li>Ensure the format is suitable to store large quantities of data.</li>
</ul>

<h4 id="specification-for-dissemination-information-packages-e-ark-dip">Specification for Dissemination Information Packages (E-ARK DIP)</h4>
<p>The main aims of this specification are to:</p>

<ul>
  <li>Define a generic structure of the DIP format suitable for a wide variety of archival records, such as document and image collections, databases or geographical data.</li>
  <li>Recommend a set of metadata related to the structural and access aspects of the DIP.</li>
</ul>

<h4 id="content-information-type-specifications-e-ark-cits">Content Information Type Specifications (E-ARK CITS)</h4>
<p>The main aim of a Content Information Type Specification (CITS) is to:</p>

<ul>
  <li>Define, in technical terms, how data and metadata must be formatted and placed within a CSIP Information Package to achieve interoperability in exchanging specific Content Information.</li>
</ul>

<p>The number of possible Content Information Type Specifications is unlimited. For a list of existing Content Information Type Specifications see the relevant section in the Common Specification for Information Packages.</p>

<h2 id="ii-organisational-support">II. Organisational Support</h2>
<p>This specification is maintained by the Digital Information LifeCycle Interoperability Standards Board (DILCIS Board, <a href="http://dilcis.eu/">http://dilcis.eu/</a>). The role of the DILCIS Board is to enhance and maintain the draft specifications developed in the European Archival Records and Knowledge Preservation Project (E-ARK project, <a href="http://eark-project.com/">http://eark-project.com/</a>) which concluded in January 2017. The Board consists of eight members, but no restriction is placed on the number of participants taking part in the work. All Board documents and specifications are stored in GitHub (<a href="https://github.com/DILCISBoard/">https://github.com/DILCISBoard/</a>) while published versions are made available on the Board webpage. Since 2018 the DILCIS Board has been responsible for the core specifications in the Connecting Europe Facility eArchiving Building Block <a href="https://ec.europa.eu/cefdigital/wiki/display/CEFDIGITAL/eArchiving/">https://ec.europa.eu/cefdigital/wiki/display/CEFDIGITAL/eArchiving/</a>.</p>

<h2 id="iii-authors--revision-history">III. Authors &amp; Revision History</h2>
<p>A full list of contributors to this specification, as well as the revision history can be found in the <a href="#postface">Postface material</a>.</p>

<h1 id="e-ark-csip">E-ARK CSIP</h1>

<h2 id="common-specification-for-information-packages-1">Common Specification for Information Packages</h2>

<p>Version: 2.0.4</p>

<p>Date: 12.06.2020</p>

<p>1.  <a href="#introduction">Introduction</a><br>
1.1.  <a href="#thecommonspecificationforinformationpackagesandoais">The Common Specification for Information Packages and OAIS</a><br>
1.2.  <a href="#thecommonspecificationforinformationpackagesandcontentinformationtypespecifications">The Common Specification for Information Packages and Content Information Type Specifications</a><br>
1.3.  <a href="#commonspecificationforinformationpackagesoaisinformationpackages%E2%80%99specificationsandcontentinformationtypespecifications">Common Specification for Information Packages, OAIS Information Packages’ specifications and Content Information Type Specifications</a><br>
1.4.  <a href="#relationtootherdocuments">Relation to other documents</a><br>
1.4.1.  <a href="#internationalstandardsandbest-practices">International standards and best-practices</a><br>
1.4.2.  <a href="#othere-arkspecifications">Other E-ARK specifications</a><br>
1.5.  <a href="#structureofthedocument">Structure of the document</a><br>
2.  <a href="#needforestablishingcommonground">Need for establishing common ground</a><br>
3.  <a href="#principlesforinteroperableinformationpackages">Principles for interoperable Information Packages</a><br>
3.1.  <a href="#generalprinciples">General principles</a><br>
3.1.1.  <a href="#principle1.1">Principle 1.1</a><br>
3.1.2.  <a href="#principle1.2:">Principle 1.2:</a><br>
3.1.3.  <a href="#principle1.3">Principle 1.3</a><br>
3.1.4.  <a href="#principle1.4:">Principle 1.4:</a><br>
3.1.5.  <a href="#principle1.5:">Principle 1.5:</a><br>
3.1.6.  <a href="#principle1.6:">Principle 1.6:</a><br>
3.1.7.  <a href="#principle1.7:">Principle 1.7:</a><br>
3.2.  <a href="#identificationoftheinformationpackage">Identification of the Information Package</a><br>
3.2.1.  <a href="#principle2.1:">Principle 2.1:</a><br>
3.2.2.  <a href="#principle2.2:">Principle 2.2:</a><br>
3.2.3.  <a href="#principle2.3:">Principle 2.3:</a><br>
3.2.4.  <a href="#principle2.4:">Principle 2.4:</a><br>
3.2.5.  <a href="#principle2.5:">Principle 2.5:</a><br>
3.3.  <a href="#structureoftheinformationpackage">Structure of the Information Package</a><br>
3.3.1.  <a href="#principle3.1:">Principle 3.1:</a><br>
3.3.2.  <a href="#principle3.2:">Principle 3.2:</a><br>
3.3.3.  <a href="#principle3.3:">Principle 3.3:</a><br>
3.3.4.  <a href="#principle3.4:">Principle 3.4:</a><br>
3.3.5.  <a href="#principle3.5:">Principle 3.5:</a><br>
3.3.6.  <a href="#principle3.6:">Principle 3.6:</a><br>
3.4.  <a href="#informationpackagemetadata">Information Package Metadata</a><br>
3.4.1.  <a href="#principle4.1:">Principle 4.1:</a><br>
3.4.2.  <a href="#principle4.2:">Principle 4.2:</a><br>
3.4.3.  <a href="#principle4.3:">Principle 4.3:</a><br>
4.  <a href="#csipstructure">CSIP structure</a><br>
4.1.  <a href="#folderstructureofthecsip">Folder structure of the CSIP</a><br>
4.2.  <a href="#implementingthestructure">Implementing the structure</a><br>
5.  <a href="#useofmetadata">Use of metadata</a><br>
5.1.  <a href="#generalrequirementsformetadatainacsipinformationpackage">General requirements for metadata in a CSIP Information Package</a><br>
5.2.  <a href="#generalrequirementsfortheuseofmetadata">General requirements for the use of metadata</a><br>
5.2.1.  <a href="#theuseofidentifiers">The use of identifiers</a><br>
5.2.2.  <a href="#referencingbetweenfileswithinacsipinformationpackage">Referencing between files within a CSIP Information Package</a><br>
5.2.3.  <a href="#referencingotherpackages">Referencing other packages</a><br>
5.2.4.  <a href="#examples">Examples</a><br>
5.3.  <a href="#useofmets">Use of METS</a><br>
5.3.1.  <a href="#useofthemetsrootelementelementmets">Use of the METS root element (element mets)</a><br>
5.3.1.1.  <a href="#locationofxmlschema">Location of XML schema</a><br>
5.3.2.  <a href="#useofthemetsheaderelementmetshdr">Use of the METS header (element metsHdr)</a><br>
5.3.3.  <a href="#useofthemetsdescriptivemetadatasectionelementdmdsec">Use of the METS descriptive metadata section (element dmdSec)</a><br>
5.3.4.  <a href="#useofthemetsadministrativemetadatasectionelementamdsec">Use of the METS administrative metadata section (element amdSec)</a><br>
5.3.5.  <a href="#useofthemetsfilesectionelementfilesec">Use of the METS file section (element fileSec)</a><br>
5.3.6.  <a href="#useofthemetsstructuralmap%60&lt;structmap&gt;%60">Use of the METS structural map (<code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code>)</a><br>
5.4.  <a href="#useofpremis">Use of PREMIS</a><br>
5.4.1.  <a href="#vocabularies">Vocabularies</a><br>
5.4.2.  <a href="#identifiers">Identifiers</a><br>
6.  <a href="#implementationconsiderations">Implementation Considerations</a><br>
6.1.  <a href="#contentinformationtypespecifications">Content Information Type Specifications</a><br>
6.1.1.  <a href="#whatisacontentinformationtypespecification?">What is a Content Information Type Specification?</a><br>
6.1.2.  <a href="#maintainingcontentinformationtypespecifications">Maintaining Content Information Type Specifications</a><br>
6.2.  <a href="#handlinglargepackages">Handling large packages</a><br>
6.2.1.  <a href="#handlingdescriptivemetadatawithinthecommonspecification">Handling descriptive metadata within the Common Specification</a><br>
7.  <a href="#appendices">Appendices</a><br>
7.1.  <a href="#appendixa:e-arkinformationpackagemetsexamples">Appendix A: E-ARK Information Package METS examples</a><br>
7.2.  <a href="#appendixb:externalschema">Appendix B: External Schema</a><br>
7.2.1.  <a href="#e-arkcsipmetsextension">E-ARK CSIP METS Extension</a><br>
7.2.2.  <a href="#premis">PREMIS</a><br>
7.3.  <a href="#appendixc:externalvocabularies">Appendix C: External Vocabularies</a><br>
7.3.1.  <a href="#contentinformationtypespecification">Content information type specification</a><br>
7.3.2.  <a href="#contentcategory">Content Category</a><br>
7.3.3.  <a href="#oaispackagetype">OAIS Package type</a><br>
7.3.4.  <a href="#notetype">Note type</a><br>
7.3.5.  <a href="#otheragenttype">Other agent type</a><br>
7.3.6.  <a href="#identifiertype">Identifier type</a><br>
7.3.7.  <a href="#dmdsecstatus">dmdSec status</a><br>
7.3.8.  <a href="#ianamediatypes">IANA media types</a><br>
7.3.9.  <a href="#filegroupnames">File group names</a><br>
7.3.10.  <a href="#structuralmaptyping">Structural map typing</a><br>
7.3.11.  <a href="#structuralmaplabel">Structural map label</a><br>
7.4.  <a href="#appendixd:afulllistofe-arkcsiprequirements">Appendix D: A Full List of E-ARK CSIP Requirements</a><br>
7.4.1.  <a href="#structuralrequirements">Structural Requirements</a><br>
7.4.2.  <a href="#metadatarequirements">Metadata Requirements</a></p>

<p><a name="introduction"></a></p>

<h1 id="1-introduction">1. Introduction</h1>
<p>This document introduces the concept of the Common Specification for Information Packages (CSIP). Its three main purposes are to:</p>

<ol>
  <li>
    <p>Establish a common understanding of the requirements which need to be met in order to achieve interoperability of Information Packages;</p>
  </li>
  <li>
    <p>Establish a common base for the development of more specific Information Package definitions and tools within the digital preservation community;</p>
  </li>
  <li>
    <p>Propose the details of an XML-based implementation of the requirements using, to the largest possible extent, standards which are widely used in international digital preservation.</p>
  </li>
</ol>

<p>Ultimately the goal of the Common Specification for Information Packages is to provide a level of interoperability between Information Packages so that tools implementing the CSIP can be taken up by institutions without the need for major modifications or adaptations.</p>

<p><a name="thecommonspecificationforinformationpackagesandoais"></a></p>

<h2 id="11-the-common-specification-for-information-packages-and-oais">1.1. The Common Specification for Information Packages and OAIS</h2>
<p>The OAIS framework defines three types of Information Packages (IPs) present in the digital preservation ecosystem: Submission Information Packages (SIPs), Archival Information Packages (AIPs) and Dissemination Information Packages (DIPs) (<a href="#fig1">Figure 1</a>). These three IP types are respectively used to submit data and metadata to digital repositories, store it in long-term preservation facilities, and deliver it to consumers.</p>

<p><a name="fig1"></a>
<img src="figs/fig_1_oais_ele_ip.svg" alt="OAIS Entities" title="OAIS Functional Entities and Information Packages"></p>

<p><strong>Figure 1:</strong> OAIS Functional Entities and Information Packages</p>

<p>The main goal in the development of this specification has been to identify and standardise the common aspects of IPs which are equally relevant and implemented by any of the functional entities of the overall digital preservation process presented in OAIS (i.e. pre-ingest, ingest, archival storage, data management and access). The practical implementation is that the specification allows for the development of generic tools and code libraries which can either be applied commonly across the whole lifecycle of digital data, or be reused as the basis for developing more specific, content or process-aware tools.</p>

<p>Process level interoperability requires detailed technical specifications for the OAIS information package types, i.e. SIP, AIP and DIP. The Common Specification for Information Packages is accompanied by corresponding extending implementation specifications for E-ARK SIP, E-ARK AIP and E-ARK DIP.</p>

<p><a name="fig2"></a>
<img src="figs/fig_2_csip_scope.svg" alt="CS SCOPE" title="The scope of Common Specification for Information Packages in regard to OAIS Information Packages."></p>

<p><strong>Figure 2:</strong> The scope of Common Specification for Information Packages in regard to OAIS Information Packages.</p>

<p>In general, the E-ARK SIP and E-ARK DIP specifications reuse and apply fully all the requirements set in this Common Specification. However, they also extend it with aspects relevant only for the respective processes (<a href="#fig2">Figure 2</a>).</p>

<p>For example, the E-ARK SIP specification extends the CSIP with further requirements about recording relevant information on a submission agreement and the actors of the submission process. On the other hand, the E-ARK DIP provides possibilities for describing complex access environments needed to reuse the content of a DIP.</p>

<p>It is important to note that the E-ARK AIP format does not extend the CSIP in the same way the E-ARK SIP and E-ARK DIP formats do, i.e. in the sense of a format specification inheriting all general properties from the CSIP which is then augmented by specific AIP requirements. The reason for this is that while the SIP and the DIP are like “snapshots” in time – one capturing the state of an information package at the time of submission (SIP), the other one capturing one form of delivery of the information for access (DIP) – then the AIP needs to deal with an “evolving object” which is constantly updated by preservation actions undertaken in the course of the object’s lifecycle. As such, while the E-ARK AIP specification does implement all of the core metadata requirements defined in the Common Specification and extends these (for example it describes a means to record preservation actions about the IP), it does also extend the default structure of the CSIP (defined in <a href="#csipstructure">Section 4</a>). Essentially the AIP introduces a more complex structure which allows at the same time to securely hold an E-ARK SIP (which itself follows in full the CSIP) and at the same time add and modify additional representations over a series of preservation actions.</p>

<p><a name="thecommonspecificationforinformationpackagesandcontentinformationtypespecifications"></a></p>

<h2 id="12-the-common-specification-for-information-packages-and-content-information-type-specifications">1.2. The Common Specification for Information Packages and Content Information Type Specifications</h2>
<p>As an interoperability standard, it must be possible to use the CSIP regardless of the type and format of the content users need to handle. At the same time, each individual content type and file format can have specific characteristics which need to be taken into account for purposes of validation, preservation and curation.</p>

<p>E-ARK specifications introduce the concept of Content Information Type Specifications to facilitate such in-depth control over specific content types and formats. A Content Information Type Specification can include detailed requirements as to how content, metadata, and documentation for specific content types (for example relational databases or geospatial data) have to be handled within a CSIP (or E-ARK SIP, AIP or DIP).</p>

<p>As of May 2019 these Content Information Type Specifications, created by the E-ARK project and enhanced by the DILCIS Board, have been verified for usage within the Common Specification for Information Packages:</p>

<ul>
  <li>
    <p>E-ARK Content Information Type Specification for ERMS: This Content Information Type Specification describes the use of the CSIP for archival records exported from ERMS-type systems (<a href="https://github.com/DILCISBoard/E-ARK-ERMS">https://github.com/DILCISBoard/E-ARK-ERMS</a>);</p>
  </li>
  <li>
    <p>E-ARK Content Information Type Specification for Geospatial data: This Content Information Type Specification builds upon the INSPIRE directive and describes the storage of geospatial information within a CSIP compatible Information Package (<a href="https://github.com/DILCISBoard/E-ARK-Geodata">https://github.com/DILCISBoard/E-ARK-Geodata</a>);</p>
  </li>
  <li>
    <p>E-ARK Content Information Type Specification for Relational Databases (SIARD1, SIARD2 and SIARDDK): This Content Information Type Specification describes the use of the CSIP for the archiving, preservation and reuse of relational databases using one of the SIARD family (Software Independent Archiving of Relational Databases) formats, (<a href="https://github.com/DILCISBoard/SIARD">https://github.com/DILCISBoard/SIARD</a>). Note, that SIARD1 and SIARDDK specifications are deemed outdated at the time of writing and are only for use when working with existing SIARD1 and SIARDDK packages within CSIP compatible Information Packages. We recommend using the SIARD2 format and the appropriate Content Information Type Specification when creating new archival packages for relational databases.</p>
  </li>
</ul>

<p><a name="fig3"></a>
<img src="figs/fig_3_csip_types.svg" alt="TYPE SPECS" title="Common Specification for Information Packages and Content Information Type Specifications."></p>

<p><strong>Figure 3:</strong> Common Specification for Information Packages and Content Information Type Specifications</p>

<p>The total number of Content Information Type Specifications is unlimited, and the long-term commitment of the DILCIS Board is to keep the overall environment open and inclusive. As such, interested bodies are welcome to develop their own Content Information Type Specifications, for example, for 3D building projects or electronic publications. An appropriate management regime to facilitate the creation and approval of additional Content Information Type Specifications by anyone in the broader community is implemented by the DILCIS Board.</p>

<p>For more detailed information about the Content Information Type Specifications see <a href="#contentinformationtypespecifications">Section 6.1</a> below and check <a href="http://www.dilcis.eu">http://www.dilcis.eu</a>.</p>

<p><a name="commonspecificationforinformationpackagesoaisinformationpackages%E2%80%99specificationsandcontentinformationtypespecifications"></a></p>

<h2 id="13-common-specification-for-information-packages-oais-information-packages-specifications-and-content-information-type-specifications">1.3. Common Specification for Information Packages, OAIS Information Packages’ specifications and Content Information Type Specifications</h2>

<p>The overall ecosystem of the E-ARK Common Specifications consists of three layers (<a href="#fig4">Figure 4</a>):</p>

<ul>
  <li>
    <p>The current document, the Common Specification for Information Packages, is the core which provides guidance which must be followed regardless of the process, data or lifecycle stage;</p>
  </li>
  <li>
    <p>The E-ARK SIP, AIP and DIP build on the CSIP and extend it with specific process-related aspects;</p>
  </li>
  <li>
    <p>The Content Information Type Specifications define detailed requirements for embedding and describing specific content types within a CSIP.</p>
  </li>
</ul>

<p><a name="fig4"></a>
<img src="figs/fig_4_cs_vs_ip.svg" alt="TYPE SPECS" title="Relations between the Common Specification for Information Packages; E-ARK SIP, AIP and DIP specifications; and Content Information Type Specifications."></p>

<p><strong>Figure 4:</strong> The relationship between the Common Specification for Information Packages; E-ARK SIP, AIP and DIP specifications; and Content Information Type Specifications</p>

<p>Therefore the “thing encountered in the wild” is the E-ARK SIP, AIP or DIP including data according to one or many Content Information Type Specifications.</p>

<p><a name="relationtootherdocuments"></a></p>

<h2 id="14-relation-to-other-documents">1.4. Relation to other documents</h2>
<p>This Common Specification for Information Packages is related to the following documents:</p>

<p><a name="internationalstandardsandbest-practices"></a></p>

<h3 id="141-international-standards-and-best-practices">1.4.1. International standards and best-practices</h3>
<ul>
  <li>
    <p>Reference Model for an Open Archival Information System (OAIS), 2012, <a href="https://public.ccsds.org/Pubs/650x0m2.pdf">https://public.ccsds.org/Pubs/650x0m2.pdf</a>
This specification uses the same terminology as introduced in the OAIS model and also the same division of information package types: Submission Information Package (SIP), Archival Information Package (AIP) and Dissemination Information Package (DIP).</p>
  </li>
  <li>
    <p>Producer-Archive Interface Specification (PAIS) – CCSDS, 2014, <a href="https://public.ccsds.org/Pubs/651x1b1.pdf">https://public.ccsds.org/Pubs/651x1b1.pdf</a>
The structure of a SIP presented in PAIS has been investigated, but because the implementation of this specification is not very comprehensive yet (only a few prototypes exist), it was decided to rely mainly on the best practices introduced in other reports (see below).</p>
  </li>
</ul>

<p><a name="othere-arkspecifications"></a></p>

<h3 id="142-other-e-ark-specifications">1.4.2. Other E-ARK specifications</h3>

<ul>
  <li>E-ARK SIP Specification (<a href="https://github.com/DILCISBoard/E-ARK-SIP">https://github.com/DILCISBoard/E-ARK-SIP</a>)</li>
  <li>E-ARK AIP Specification (<a href="https://github.com/DILCISBoard/E-ARK-AIP">https://github.com/DILCISBoard/E-ARK-AIP</a>)</li>
  <li>E-ARK DIP Specification (<a href="https://github.com/DILCISBoard/E-ARK-DIP">https://github.com/DILCISBoard/E-ARK-DIP</a>)</li>
</ul>

<p>The E-ARK SIP, AIP and DIP specifications build on the Common Specification for
Information Packages and extend it in regard to requirements derived from pre-ingest and ingest, archival storage and access processes.</p>

<p><a name="structureofthedocument"></a></p>

<h2 id="15-structure-of-the-document">1.5. Structure of the document</h2>
<p>The rest of this document describes the CSIP and its practical implementation. The document is divided into two logical parts.</p>

<p>The first part (<a href="#needforestablishingcommonground">Section 2</a> and <a href="#principlesforinteroperableinformationpackages">Section 3</a>) describes the generic principles of the CSIP. The main aim of these Sections is to first identify a common set of needs and thereafter present a series of requirements which an Information Package needs to follow regardless of the implementation at any given point in time:</p>

<ul>
  <li>
    <p><a href="#needforestablishingcommonground">Section 2</a> provides an explanation of the need for a CSIP. The section presents some practical use cases which highlight the potential savings and increased functionality of digital archives when following internationally standardised approaches.</p>
  </li>
  <li>
    <p><a href="#principlesforinteroperableinformationpackages">Section 3</a> presents the core principles which need to be met in order to achieve the interoperability goal described in Section 2. Based on these requirements a set of high-level solutions are introduced regarding, for example, the structure and use of metadata within any implementation of an Information Package.</p>
  </li>
</ul>

<p>The second part of this document (<a href="#csipstructure">Section 4</a>, <a href="#useofmetadata">Section 5</a> and <a href="#implementationconsiderations">Section 6</a>) presents a practical implementation of the principles described in previous Sections, as implemented according to current state-of-the-art technologies. As such, this part of the document describes the requirements which are needed to achieve practical IP interoperability:</p>

<ul>
  <li>
    <p><a href="#csipstructure">Section 4</a> presents a detailed description of the structure which must be implemented in any CSIP
Information Package.</p>
  </li>
  <li>
    <p><a href="#useofmetadata">Section 5</a> presents a detailed overview of metadata requirements within CSIP Information Packages with a special focus on the use of metadata elements which are needed for the automation and interoperability of archival validation and identification tasks.</p>
  </li>
  <li>
    <p><a href="#implementationconsiderations">Section 6</a> describes additional (optional) components extending the practical implementation in regard to specific aspects:</p>
    <ul>
      <li>How to create new Content Information Type Specifications</li>
      <li>How to split large content objects between multiple physical IPs</li>
      <li>Generic guidelines on adding (any) descriptive metadata into a CSIP Information Package</li>
    </ul>
  </li>
</ul>

<p>Finally, in addition to this document, full examples of IPs conforming to the Common Specification for Information implementation details are available in <a href="/examples/">the examples directory on this site</a>.</p>

<p><a name="needforestablishingcommonground"></a></p>

<h1 id="2-need-for-establishing-common-ground">2. Need for establishing common ground</h1>

<p><strong>The vision:</strong> <em>All digital preservation systems receive, store and provide access to information, regardless of its size, type or format, according to a set of agreed principles which allow institutions to identify, verify and validate the information in a uniform way.</em></p>

<p><strong>The goal:</strong> <em>Interoperability between data sources, archives and reuse environments is improved to a point where digital preservation tools can be reused across borders and institutions. This opens up new possibilities for collaboration and reduces the need for development resources for any single institution.</em></p>

<p>The amount of digital information being created, held and exchanged is continuously growing. This information is created with the help of numerous software tools and systems, comes in a variety of technical formats, and covers most aspects of our daily lives. Regardless of the formats and systems in question, it is necessary to consider whether the information needs to be retained and managed for longer periods of time. The reasons for this might be, for example:</p>

<ul>
  <li>to meet legal and regulatory obligations</li>
  <li>to provide for efficient reuse</li>
  <li>to satisfy historical, cultural, scientific and business interest.</li>
</ul>

<p>Currently, most tools and systems used to create information are not built for coping with long-term
requirements for keeping information safe and accessible. Instead, implementations separate the short-term and long-term management of information into different systems, for example, business and records
systems on one hand and archival systems on the other (<a href="#fig5">Figure 5</a>).</p>

<p><a name="fig5"></a>
<img src="figs/fig_5_oais_ent.svg" alt="OAIS Entities" title="Information flow between live and archival systems"></p>

<p><strong>Figure 5:</strong> Information flow between live and archival systems</p>

<p>The implication for data owners and system managers is that information which has to be kept for
extended time periods need to be exchanged between a set of different locations, including archival
systems:</p>

<ul>
  <li>as effectively as possible,</li>
  <li>without endangering the authenticity and integrity of the information,</li>
  <li>and without limiting the possibilities for discovering and reusing the information.</li>
</ul>

<p>As such, what is needed to make the long-term availability of crucial information possible under
(usually limited) resources is a set of principles which allow exchanging information in a common way
across the systems participating in archival workflows and processes (i.e. create a set of interoperability
specifications). For archival information packages, the following interoperability scenarios have been identified
(<a href="#fig6">Figure 6</a>):</p>

<ul>
  <li>Export of data and metadata from source systems and transfer to SIP creation tools (or directly, as
a SIP, into preservation systems);</li>
  <li>Transfer of SIPs from SIP creation tools to preservation systems;</li>
  <li>Exchange of preservation systems where all AIPs need to be transferred (ingested) into a new
technological platform;</li>
  <li>Distributed storage and synchronisation of AIPs between multiple (technologically different)
preservation systems;</li>
  <li>Exchange of DIPs between preservation systems and access platforms or portals;</li>
  <li>Exchange of DIPs between various access platforms of portals.</li>
</ul>

<p><a name="fig6"></a>
<img src="figs/fig_6_arch_wrkflw.svg" alt="OAIS Entities" title="Archival workflow and tool ecosystem"></p>

<p><strong>Figure 6:</strong> Archival workflow and tool ecosystem</p>

<p>As of 2014 (the start of the development of this specification), the state of interoperability in digital preservation was rather poor. While national and institutional practical implementation-level specifications existed to serve the need for data and metadata packaging and exchange, these were generally not interoperable with each other. On the contrary, available and widely used international specifications (most notably METS and PREMIS) lack the necessary implementation-level detail, needed to serve as an authoritative source for practical interoperability.</p>

<p>This situation has a remarkable effect on the cost of digital preservation. Namely, the tools developed in individual institutions are not reusable across institutional and state borders and therefore need to be redeveloped at each location. Globally, this raises the cost of digital preservation to a level which makes it unaffordable for smaller institutions and, at the same time, does often not allow for developing tools which would be sufficiently mature, user-friendly and not prone to errors. Furthermore, the multitude of national or institutional specifications does not allow internationally active source system providers (e.g. Oracle, Microsoft) to build a single native archiving functionality into their products, meaning that there is a need for bespoke development (and therefore added cost) for each installation of these source systems across all sectors and countries.</p>

<p>To overcome these limitations this document proposes a universal common specification, which can be implemented across borders, describing how data and metadata should be structured and packaged when transferred to archival systems, ingested and preserved in these, and re-used. Such a specification will allow data owners to build standardised interfaces for the export of their data regardless of the archives in question; and digital archives to build standardised interfaces for data ingest and access, regardless of the data providers and users in question.</p>

<p>Further, the aim of the common specification is to be sufficiently detailed and technical to allow for extended collaboration in regard to software development and pooling. Ideally the tools which implement the common specification for data export, transfer, ingest, preservation and reuse are exchangeable between institutions and administrations with minimal effort. This leads to a significant decrease in resources needed from any single institution and opens up an extended market for commercial software providers.</p>

<p><a name="principlesforinteroperableinformationpackages"></a></p>

<h1 id="3-principles-for-interoperable-information-packages">3. Principles for interoperable Information Packages</h1>
<p>At the heart of any standardisation activity has to be a clear understanding of the needs and aims which have to be addressed. This is also the goal of this section, which presents a series of high-level principles to guide the technical details delivered in Part II of this specification.</p>

<p>Most of the principles are driven by the aim of interoperability, which is that Information Packages shall be easy to exchange, identify, validate and (re)use with a wide variety of software tools and systems.</p>

<p>Another crucial factor to take into account is long-term sustainability. Practical technical and semantic interoperability is possible only when a certain set of technologies have been agreed upon and implemented. However, any technology will become outdated sooner or later, and previously agreed-upon approaches have to be updated to accommodate new, better and more efficient technologies and standards. Because of this, the developers of this Common Specification for Information Packages have reused, as much as possible, existing powerful, standardised and well-established best practices for the technical implementation of an Information Package (Part II of this document). This does not mean that the technical implementation details will not need to be changed in future, only that the need will arise later rather than sooner. To achieve long-term sustainability of the Common Specification for Information Packages, we present below a set of generic principles which must be followed when updating any specific implementation details at any point in time.</p>

<p>The principles present a conceptual view of an Information Package, including an overall IP data model, and use of data and metadata. An implementation of this conceptual view is presented later, in Part II of this document.</p>

<p>Each principle has a sequential number and a short description. The description always includes a MoSCoW (MUST/MUST NOT, SHOULD/SHOULD NOT, COULD, WOULD) prioritisation statement. The short description of each principle is followed by a rationale which describes the reason and background for the principle.</p>

<p><a name="generalprinciples"></a></p>

<h2 id="31-general-principles">3.1. General principles</h2>

<p><a name="principle1.1"></a></p>

<h3 id="311-principle-11">3.1.1. Principle 1.1</h3>
<p><em>It <strong>MUST</strong> be possible to include any data or metadata in an Information Package regardless of its type or format.</em></p>

<p>This is one of the most crucial principles of the CSIP. To be truly “common”, technical implementations of the CSIP MUST NOT introduce limitations or restrictions which are only applicable to certain data or metadata types. If an Information Package implementation fails to meet this principle, it is not possible to use it across different sectors and tools, thereby limiting practical interoperability.</p>

<p><a name="principle1.2:"></a></p>

<h3 id="312-principle-12">3.1.2. Principle 1.2:</h3>
<p><em>The Information Package <strong>MUST NOT</strong> restrict the means, methods or tools for exchanging it.</em></p>

<p>Tools and methods for transferring Information Packages between locations are constantly evolving. It is also possible that different methods are preferred for packages of varying sizes. To ensure that a CSIP Information Package is truly interoperable across different platforms, it MUST NOT introduce limitations or restrictions which would be impossible to be met by specific information exchange tools or channels.</p>

<p>As such, the CSIP does also not define the principle to use a particular transfer package or envelope. The scope of the CSIP is limited to the structure and requirements for data and metadata within the package. Different implementers are welcome to choose their own methods on top of the CSIP.</p>

<p><a name="principle1.3"></a></p>

<h3 id="313-principle-13">3.1.3. Principle 1.3</h3>
<p><em>The package format <strong>MUST NOT</strong> define the scope of data and metadata which constitutes an Information Package.</em></p>

<p>One of the fundamental principles of the CSIP is that it MUST allow each individual repository to define the (intellectual) scope of an Information Package and its relations to real-life entities. As such, any implementation of the CSIP MUST be equally usable for packaging, for example, the entire content of an ERMS as a single IP; or for extracting each record and its metadata from the ERMS individually and packaging each as a separate IP.</p>

<p>Out of the previous, we can also derive that a CSIP specification MUST NOT define that, for example, a SIP should conform to exactly one AIP. Instead, the CSIP MUST allow for the inclusion of “anything that the implementer wants to define as a SIP, AIP or DIP” and allow for “any relationships (1-1; 1-n; n-1; n-m) between SIPs, AIPs and DIPs”.</p>

<p><a name="principle1.4:"></a></p>

<h3 id="314-principle-14">3.1.4. Principle 1.4:</h3>
<p><em>The Information Package <strong>SHOULD</strong> be scalable.</em></p>

<p>One of the practical concerns for Information Packages is their size. Many digital repositories have problems with data objects and metadata of increasing sizes, making it especially difficult to carry out tasks related to data or metadata validation, and identification and modification. For example, Information Packages that include relational databases or born-digital 3D movies can easily reach TB sizes.</p>

<p>Consequently, any current or future implementation of the CSIP is required to provide for appropriate scalability mechanisms (for example, mechanisms for splitting large-scale data or metadata).</p>

<p><a name="principle1.5:"></a></p>

<h3 id="315-principle-15">3.1.5. Principle 1.5:</h3>
<p><em>The Information Package <strong>MUST</strong> be machine-readable</em></p>

<p>To support the goal of automating ingest, preservation and access workflows each of the implementations of the CSIP must be machine-actionable. This means that decisions about the use of metadata syntax and semantics as well as the physical structure must be expressed explicitly and in a clear way. This, in turn, allows the specification to be implemented in the same way across different tools and environments.</p>

<p><a name="principle1.6:"></a></p>

<h3 id="316-principle-16">3.1.6. Principle 1.6:</h3>
<p><em>The Information Package <strong>SHOULD</strong> be human-readable</em></p>

<p>In long-term preservation, it is necessary to take into account that “forgotten” Information Packages might be found long after details about the implementation are gone and no tools to access the package are available. For these scenarios, it is crucial to ensure that the structure and metadata of the Information Package are understandable with minimal effort by using simple tools like text editors and file viewers.</p>

<p>In practice, this means that any implementation of the CSIP should ensure that folder and file naming conventions allow for the human identification of package components and that the semantics of the package is explicit.</p>

<p><a name="principle1.7:"></a></p>

<h3 id="317-principle-17">3.1.7. Principle 1.7:</h3>
<p><em>The Information Package <strong>MUST NOT</strong> prescribe the use of a specific preservation method</em></p>

<p>Different preservation institutions and different types of data need to use different methods for long-term preservation; migration and emulation are typical examples. A CSIP implementation MUST NOT prescribe the use of a specific preservation method. Instead, it should allow users to document and/or add arbitrary data or metadata as necessary for preservation purposes.</p>

<p><a name="identificationoftheinformationpackage"></a></p>

<h2 id="32-identification-of-the-information-package">3.2. Identification of the Information Package</h2>

<p><a name="principle2.1:"></a></p>

<h3 id="321-principle-21">3.2.1. Principle 2.1:</h3>
<p><em>The Information Package OAIS type (SIP, AIP or DIP) <strong>MUST</strong> be clearly indicated.</em></p>

<p>One of the first tasks in analysing any Information Package is to identify its current status in the overall archival process. Therefore, any Information Package must explicitly and uniformly identify itself as a SIP, AIP or DIP.</p>

<p><a name="principle2.2:"></a></p>

<h3 id="322-principle-22">3.2.2. Principle 2.2:</h3>
<p><em>Any Information Package <strong>MUST</strong> clearly identify the Content Information Type(s) of its data and metadata.</em></p>

<p>As stated in Principle 1.1, any Information Package MUST be able to include any kind of data and metadata. At the same time, we have introduced in earlier Sections the concept of Content Information Types which allow users to achieve more detailed control and fine-grained interoperability. As such, any CSIP Information Package MUST include a statement about which Content Information Type Specification(s) has been followed within the Information Package, or on the contrary, indicate clearly that no specific Content Information Type Specification has been followed.</p>

<p>The practical implication of principles 1.1, 2.1 and 2.2 is that, once these have been followed in implementations, it is possible to develop modular identification and validation tools and workflows. While generic components can carry out high-level tasks regardless of the Content Information Type, it is possible to detect automatically which additional content-aware modules need to be executed.</p>

<p><a name="principle2.3:"></a></p>

<h3 id="323-principle-23">3.2.3. Principle 2.3:</h3>
<p><em>Any Information Package <strong>MUST</strong> have an identifier which is unique and persistent within the repository.</em></p>

<p>In order to manage a digital repository and provide access services, each Information Package stored in the repository MUST be identified uniquely at least within the repository. At the same time, a CSIP implementation MUST NOT limit the choice of the exact identification mechanism, as long as the mechanism is implemented consistently throughout the repository.</p>

<p><a name="principle2.4:"></a></p>

<h3 id="324-principle-24">3.2.4. Principle 2.4:</h3>
<p><em>Any Information Package <strong>SHOULD</strong> have an identifier which is globally unique and persistent.</em></p>

<p>In addition to the previous principle, it is recommended that the identification mechanism used at the repository provides for global uniqueness and persistence of Information Package IDs. The application of globally unique and persistent identifiers allows repositories to participate more easily in cross-institutional information exchange and reuse scenarios (for example participation in national or international portals, or cross-repository duplication of AIP preservation). However, the CSIP MUST NOT limit the choice of the exact identification mechanism.</p>

<p><a name="principle2.5:"></a></p>

<h3 id="325-principle-25">3.2.5. Principle 2.5:</h3>
<p><em>All components of an Information Package <strong>MUST</strong> have an identifier which is unique and persistent within the repository.</em></p>

<p>As stated above, an Information Package MUST be flexible enough to allow for the inclusion of any data or metadata depending on the needs of the repository and its users. As well, an Information Package might include additional support documentation like metadata schemas, user guidelines, contextual documentation etc. Regardless of which and how many components constitute a full Information Package, all components MUST have a unique and persistent identifier which allows for the appropriate linking of data, metadata and all other components. This, in turn, is one of the most crucial aspects for achieving an interoperable way of maintaining package integrity.</p>

<p>It is also worth mentioning that in any implementation, it is only necessary to achieve identifier uniqueness and persistence within an individual Information Package. If this is the case, repository-wide uniqueness is easily achieved when combining the package ID (unique according to principle 2.3) and the component ID.</p>

<p>The components of an Information Package are explained in more detail in the following section.</p>

<p><a name="structureoftheinformationpackage"></a></p>

<h2 id="33-structure-of-the-information-package">3.3. Structure of the Information Package</h2>

<p><a name="principle3.1:"></a></p>

<h3 id="331-principle-31">3.3.1. Principle 3.1:</h3>
<p><em>The Information Package <strong>MUST</strong> ensure that data and metadata are logically separated from one another.</em></p>

<p>At the highest level, each Information Package can be logically subdivided into data and metadata. This logical separation minimises the effort required to identify or validate content/metadata and simplifies long-term preservation actions. For example, ingest tools may implement separate, efficient metadata identification and validation tasks as opposed to content format identification and normalisation tasks. Over the lifetime of a package, this separation also facilitates long-term preservation tasks, such as partial metadata or data updates that do not put the integrity of the package at risk. Regardless of the physical structure of a package, the Information Package <strong>MUST</strong> provide logical separation of data and metadata in the package’s manifest.</p>

<p><a name="principle3.2:"></a></p>

<h3 id="332-principle-32">3.3.2. Principle 3.2:</h3>
<p><em>The Information Package <strong>SHOULD</strong> ensure that data and metadata are physically separated from one another.</em></p>

<p>In addition to the logical separation of components, it is beneficial to have data and metadata physically separated (i.e. formatted as individual computer files or clearly separated bitstreams). This allows digital preservation tools and systems to update respective data or metadata portions of an Information Package without endangering the integrity of the whole package.</p>

<p><a name="principle3.3:"></a></p>

<h3 id="333-principle-33">3.3.3. Principle 3.3:</h3>
<p><em>The structure of the Information Package <strong>SHOULD</strong> allow for the separation of different types of metadata</em></p>

<p>In addition to the previous principle, it is recommended to explicitly divide metadata into more specific components. While the definitions of metadata types vary a lot between implementations, it is recommended that metadata is divided both logically and physically at least into descriptive and preservation metadata.</p>

<p><a name="principle3.4:"></a></p>

<h3 id="334-principle-34">3.3.4. Principle 3.4:</h3>
<p><em>The structure of the Information Package <strong>MUST</strong> allow for the creation of data and metadata in multiple representations.</em></p>

<p>The concept of representations is one of the fundamental building blocks in digital preservation. As technologies evolve and become obsolete, data and metadata are constantly updated to ensure long-term accessibility, therefore creating new versions or representations of the data and metadata.</p>

<p>Expressing representations within the logical and physical structure of an Information Package helps institutions to explicitly understand the various states of the information throughout its lifecycle, therefore improving also the ease of long-term management and reuse of the information.</p>

<p><a name="principle3.5:"></a></p>

<h3 id="335-principle-35">3.3.5. Principle 3.5:</h3>
<p><em>The structure of the Information Package <strong>MUST</strong> explicitly define the possibilities for adding additional components into the Information Package.</em></p>

<p>In addition to data and metadata, institutions might need to include additional components in an Information Package. For example, implementers might decide that XML Schemas about metadata structures and additional binary documentation about the original IT environment have to be added to the package.</p>

<p>If this is the case, the CSIP Information Package MUST NOT limit which components can constitute an Information Package and MUST offer clearly defined extension points for the inclusion of these additional components into the Information Package. At the same time, these extension points MUST be defined in a way which does not interfere with other components (i.e. the extension points MUST be clearly separated from other components of an Information Package).</p>

<p><a name="principle3.6:"></a></p>

<h3 id="336-principle-36">3.3.6. Principle 3.6:</h3>
<p><em>The Information Package <strong>SHOULD</strong> follow a common conceptual structure regardless of its technical implementation.</em></p>

<p>Based on principles 3.1 – 3.5, a common structure for any CSIP Information Package is presented (<a href="#fig7">Figure 7</a>).</p>

<p><a name="fig7"></a>
<img src="figs/fig_7_cs_con_struct.svg" alt="Conceptual Structure" title="Conceptual structure of the Common Specification"></p>

<p><strong>Figure 7:</strong> Conceptual structure of the Common Specification</p>

<p>Following Principle 3.1 the package MUST include a high-level structural component for metadata which includes at least relevant metadata for the whole package. In addition, the representations MUST internally separate between data and metadata (though note that the CSIP does not mandate that both data and metadata must be available in all representations).</p>

<p>Following Principle 3.2, it is strongly recommended that this logical structure is manifested as a physical folder structure.</p>

<p>Following Principle 3.3, it is strongly recommended that any package metadata is subdivided into separate metadata sub-types.</p>

<p>Following Principle 3.4, the structure separates the representations of data and metadata explicitly into a separate structural component.</p>

<p>Following Principle 3.5, repositories and their users have the possibility to add any additional components (as an example for schemas and binary support documentation) either as extensions to the whole Information Package or into a specific representation.</p>

<p>This common structure <strong>SHOULD</strong> be followed throughout all implementations of the CSIP.</p>

<p>The conceptual structure presented above can be implemented in various ways – for example, the components might be defined by accompanying metadata or explicitly through a physical structure. However, it is not reasonable to have multiple implementations available at once as this would lead to unnecessary complexity in developing interoperable tools for creating, processing and managing Information Packages. At the time being for CSIP the highly recommended implementation is to use a fixed physical folder structure in combination with a manifest in the form of a METS-document (see Section 4 and Section 5) as the implementation of this specification.</p>

<p>At the same time, it is clear that any given technical implementation will become obsolete in time, for example, as new transfer methods and storage solutions emerge. As such this specification does not prohibit the take-up of any emerging logical or physical technical solutions.</p>

<p><a name="informationpackagemetadata"></a></p>

<h2 id="34-information-package-metadata">3.4. Information Package Metadata</h2>

<p><a name="principle4.1:"></a></p>

<h3 id="341-principle-41">3.4.1. Principle 4.1:</h3>
<p><em>Metadata in the Information Package <strong>MUST</strong> conform to a standard.</em></p>

<p>To exchange, validate, process and reuse Information Packages in an interoperable and automated way, it is necessary to standardise how crucial metadata are presented in the package. “Crucial metadata” is defined in this specification as the core information about how the package content has been created and managed (administrative and preservation metadata), explicit descriptions about of the structure of the package (structural metadata) and the technical details of the data themselves (technical metadata).</p>

<p>To ensure that these metadata are understood and implemented in a common and interoperable way in any Information Package, the use of established and widely used metadata standards is highly recommended. In the current implementation, a large proportion of such metadata is covered by the widely used METS and PREMIS standards (see Section 5).</p>

<p><a name="principle4.2:"></a></p>

<h3 id="342-principle-42">3.4.2. Principle 4.2:</h3>
<p><em>Metadata in the Information Package <strong>MUST</strong> allow for unambiguous use.</em></p>

<p>Many metadata standards support multiple options for describing specific details of an Information Package. However, such interpretation possibilities can also lead to different implementations and ultimately to the loss of interoperability.</p>

<p>To overcome this risk, the CSIP requires that, while developing a specific implementation, the chosen metadata standard MUST be reviewed regarding potential ambiguity. If needed, the selected metadata standard MUST be further refined to meet the needs of interoperability and automation.</p>

<p><a name="principle4.3:"></a></p>

<h3 id="343-principle-43">3.4.3. Principle 4.3:</h3>
<p><em>The Information Package <strong>MUST NOT</strong> restrict the addition of supplementary metadata.</em></p>

<p>Previous principles state the importance of controlled metadata for interoperability purposes. At the same time, the opposite applies for other types of metadata, most prominently for resource discovery (also called descriptive) or Content Information Type specific technical and structural metadata. So as not to limit the widespread adoption of the CSIP, it has to be possible for any implementer to add any metadata next to the mandatory metadata components needed for package-level automation and interoperability.</p>

<p>In case organisations need to prescribe further details about descriptive or Content Information Type specific metadata for a deeper level of interoperability, it is possible to use the mechanism of Content Information Type Specifications described above.</p>

<p>To summarise the requirements above from a more technical perspective, the CSIP foresees a modular approach towards Information Package metadata:</p>

<ul>
  <li>
    <p>All Information Packages share a common core of metadata which allows for the common development of high-level package creation, validation, identification and reuse tools;</p>
  </li>
  <li>
    <p>The rest of the metadata in the Information Package might follow additional agreements which have been made to develop specific tools such as, for example, tools to manage archival descriptions in EAD, or for specific Content Information Types like relational databases in the SIARD2 format.</p>
  </li>
</ul>

<p><span style="font-size:xx-large; font-style:bold;">PART II: Implementation of the CSIP</span></p>

<p>In this part of the document we present an implementation of the requirements and principles presented in Part I of the specifciation for CSIP. The implementation consists of two core elements: a fixed physical structure of a CSIP Information Package (Section 4) and the exact use of metadata using the “Metadata Encoding &amp; Transmission Standard” (METS) <a href="http://www.loc.gov/standards/mets/">http://www.loc.gov/standards/mets/</a> and “PREservation Metadata Implementation Strategies” (PREMIS) <a href="http://www.loc.gov/standards/premis/">http://www.loc.gov/standards/premis/</a> format (Section 5).</p>

<p>As explained earlier, any implementation using a metadata standard will inevitably become obsolete. However, the authors have reused available best practices and established standards, and held discussions with the digital preservation community to ensure that the implementation is as future proof as possible.</p>

<p><a name="csipstructure"></a></p>

<h1 id="4-csip-structure">4. CSIP structure</h1>
<p>The preferred implementation of the logical model described in <a href="#principle3.6:">Principle 3.6</a> is a strict physical (folder) structure that precisely follows the logical structure. While the specification does not prohibit alternative implementations of the conceptual model, the practice is not recommended.</p>

<p>The main reason for this implementation decision is that a fixed and documented folder structure makes the package layout clear to both human users and automated tools. The main benefit this clarity is that many archival tasks (e.g. file format risk analysis), can be executed directly on the data portion of the package structure, as opposed to first processing potentially large amounts of metadata for file locations. This allows for more efficient processing which is valuable in the case of large collections and bulk operations. A fixed folder structure, therefore, provides efficiency and scalability.</p>

<p>Many data storage solutions do not explicitly support folder structures, but use other means for structuring and storing AIP data and metadata. However, the purpose of this specification is to facilitate and support Information Package interoperability. When storage solutions do not support the implementation of the package structure for native AIP storage, it is still possible to implement the physical structure for SIPs and DIPs. While systems need to implement transformations between Common Specification IPs and internal AIPs it allows interoperability between tools that support the common specification, easy transfer of IPs to new repository systems or storage solutions and the establishment of multi-repository duplicated storage solutions.</p>

<p><a name="folderstructureofthecsip"></a></p>

<h2 id="41-folder-structure-of-the-csip">4.1. Folder structure of the CSIP</h2>
<p>The CSIP folder structure is presented in <a href="#fig8">Figure 8</a> below. The structure directly follows the principles of the conceptual data model, dividing the package components into individual folders for representations, metadata, and other components. All of folders described <strong>ought to</strong> be present even if they are empty.</p>

<p><a name="fig8"></a>
<img src="figs/fig_8_csip_struct.svg" alt="IP Folder Structure" title="CSIP Information Package folder structure."></p>

<p><strong>Figure 8:</strong> CSIP Information Package folder structure</p>

<p>The implementation requirements of the CSIP Information Package structure are:</p>

<p><a name="CSIPSTR1"></a>
<strong>CSIPSTR1</strong>: Any Information Package <strong>MUST</strong> be included within a single physical root folder (known as the “Information Package root folder”). For packages presented in an archive format, <a href="#CSIPSTR3">see CSIPSTR3</a>, the archive <strong>MUST</strong> unpack to a single root folder.</p>

<p><a name="CSIPSTR2"></a>
<strong>CSIPSTR2</strong>: The Information Package root folder <strong>SHOULD</strong> be named with the ID or name of the Information Package, that is the value of the package METS.xml’s root <code class="language-plaintext highlighter-rouge">&lt;mets&gt;</code> element’s <code class="language-plaintext highlighter-rouge">@OBJID</code> attribute.</p>

<p><a name="CSIPSTR3"></a>
<strong>CSIPSTR3</strong>: The Information Package root folder <strong>MAY</strong> be compressed (for example by using TAR or ZIP). Which specific compression format to use needs to be stated in the Submission Agreement.</p>

<p><a name="CSIPSTR4"></a>
<strong>CSIPSTR4</strong>: The Information Package root folder <strong>MUST</strong> include a file named <code class="language-plaintext highlighter-rouge">METS.xml</code>. This file <strong>MUST</strong> contain metadata that identifies the package, provides a high-level package description, and describes its structure, including pointers to constituent representations.</p>

<p><a name="CSIPSTR5"></a>
<strong>CSIPSTR5</strong>: The Information Package root folder <strong>SHOULD</strong> include a folder named <code class="language-plaintext highlighter-rouge">metadata</code>, which SHOULD include metadata relevant to the whole package.</p>

<p><a name="CSIPSTR6"></a>
<strong>CSIPSTR6</strong>: If preservation metadata are available, they <strong>SHOULD</strong> be included in sub-folder <code class="language-plaintext highlighter-rouge">preservation</code>.</p>

<p><a name="CSIPSTR7"></a>
<strong>CSIPSTR7</strong>: If descriptive metadata are available, they <strong>SHOULD</strong> be included in sub-folder <code class="language-plaintext highlighter-rouge">descriptive</code>.</p>

<p><a name="CSIPSTR8"></a>
<strong>CSIPSTR8</strong>: If any other metadata are available, they <strong>MAY</strong> be included in separate sub-folders, for example an additional folder named <code class="language-plaintext highlighter-rouge">other</code>.</p>

<p><a name="CSIPSTR9"></a>
<strong>CSIPSTR9</strong>: The Information Package folder <strong>SHOULD</strong> include a folder named <code class="language-plaintext highlighter-rouge">representations</code>.</p>

<p><a name="CSIPSTR10"></a>
<strong>CSIPSTR10</strong>: The <code class="language-plaintext highlighter-rouge">representations</code> folder <strong>SHOULD</strong> include a sub-folder for each individual representation (i.e. the “representation folder”). Each representation folder should have a string name that is unique within the package scope. For example the name of the representation and/or its creation date might be good candidates as a representation sub-folder name.</p>

<p><a name="CSIPSTR11"></a>
<strong>CSIPSTR11</strong>: The representation folder <strong>SHOULD</strong> include a sub-folder named <code class="language-plaintext highlighter-rouge">data</code> which <strong>MAY</strong> include all data constituting the representation.</p>

<p><a name="CSIPSTR12"></a>
<strong>CSIPSTR12</strong>: The representation folder <strong>SHOULD</strong> include a metadata file named <code class="language-plaintext highlighter-rouge">METS.xml</code> which includes information about the identity and structure of the representation and its components. The recommended best practice is to always have a <code class="language-plaintext highlighter-rouge">METS.xml</code> in the representation folder.</p>

<p><a name="CSIPSTR13"></a>
<strong>CSIPSTR13</strong>: The representation folder <strong>SHOULD</strong> include a sub-folder named <code class="language-plaintext highlighter-rouge">metadata</code> which <strong>MAY</strong> include all metadata about the specific representation.</p>

<p><a name="CSIPSTR14"></a>
<strong>CSIPSTR14</strong>: The Information Package <strong>MAY</strong> be extended with additional sub-folders.</p>

<p><a name="CSIPSTR15"></a>
<strong>CSIPSTR15</strong>: We recommend including all XML schema documents for any structured metadata within package. These schema documents <strong>SHOULD</strong> be placed in a sub-folder called <code class="language-plaintext highlighter-rouge">schemas</code> within the Information Package root folder and/or the representation folder.</p>

<p><a name="CSIPSTR16"></a>
<strong>CSIPSTR16</strong>: We recommend including any supplementary documentation for the package or a specific representation within the package. Supplementary documentation <strong>SHOULD</strong> be placed in a sub-folder called <code class="language-plaintext highlighter-rouge">documentation</code> within the Information Package root folder and/or the representation folder.</p>

<p><a name="implementingthestructure"></a></p>

<h2 id="42-implementing-the-structure">4.2. Implementing the structure</h2>
<p>The requirements presented in Section 4.1 leave scope for decisions during the implementation. For clarity we provide two extreme examples – both the simplest and the most complete use of the structure.</p>

<p>In the simple case the structure can be implemented for the most part by adhering to only the MUST requirements. An example of this is shown in <a href="#fig9">Figure 9</a>.</p>

<p><a name="fig9"></a>
<img src="figs/fig_9_csip_simple.svg" alt="CSIP Example" title="A simple CSIP structure example."></p>

<p><strong>Figure 9:</strong> A simple CSIP structure example.</p>

<p>Note that the representations have been kept as simple as possible. All metadata for both the package and the representations (METS, EAD and
PREMIS metadata) are located in the Information Package folder rather than in the representation folders.</p>

<p>Such a simple implementation is reasonable in scenarios where the amount of data and metadata is limited. However, in the case of large Information Packages (e.g. packages comprising several representations, each with 1,000,000 files) the size of both the <code class="language-plaintext highlighter-rouge">METS.xml</code> file and preservation metadata can become too large to manage efficiently. In such large data scenarios it might prove necessary to implement all the features of the structure presented in the previous Section.</p>

<p>An example of a full implementation is illustrated in <a href="#fig10">Figure 10</a>. One observation is that the representations of the complete example essentially repeat the simple structure. Structural and preservation metadata in METS and PREMIS formats are available in both the Information Package folder, package level metadata, and the representation folders, representation level metadata. This illustrates how the full structure facilitates the management of single representations bringing benefits such as simpler metadata versioning. It is worth noting, to avoid confusion, that we recommend adoption of a common approach, either adding metadata to representations or not. That is, we recommend placing all representation-relevant metadata in a single location. You may use either the package level metadata folder or the representation level metadata folder, but do not divide metadata between the two inconsistently, with representation metadata stored at both package and representation level. We also do not recommend duplication of metadata or content of optional folders, e.g. schemas, documentation, etc., between the Information Package folder and representation folders.</p>

<p><a name="fig10"></a>
<img src="figs/fig_10_csip_full.svg" alt="CSIP Example" title="Example of the full use of the CSIP structure."></p>

<p><strong>Figure 10:</strong> Example of the full use of the CSIP structure
 </p>

<p><a name="useofmetadata"></a></p>

<h1 id="5-use-of-metadata">5. Use of metadata</h1>

<p><a name="generalrequirementsformetadatainacsipinformationpackage"></a></p>

<h2 id="51-general-requirements-for-metadata-in-a-csip-information-package">5.1. General requirements for metadata in a CSIP Information Package</h2>
<p>The primary consideration with metadata is, as with the rest of this specification, interoperability. Specifically, the high-level technical interoperability and tasks that allow an Information Package to be prepared, transferred and received, regardless of the institutions or tools involved. These tasks include:</p>

<ul>
  <li>Uniquely identifying an Information Package and its components;</li>
  <li>Validating an Information Package and its contents;</li>
  <li>Establishing the authenticity of the Information Package;</li>
  <li>Accessing the contents of an Information Package.</li>
</ul>

<p>In technical terms, the CSIP tries to control metadata needed by tools or users to:</p>

<ul>
  <li>navigate data and metadata components within the package (i.e. packaging metadata);</li>
  <li>validate that no component has been damaged during transfer or preservation (i.e. fixity information);</li>
  <li>understand the processes used when creating and managing the package (i.e. provenance and preservation metadata); and</li>
  <li>understand how the data within the package can be accessed (i.e. representation information).</li>
</ul>

<p>Descriptive metadata and most detailed technical metadata is outside the scope of the CSIP. As such, the CSIP does not provide detailed semantic interoperability between different systems. However, as noted in Section 1.2, implementers are welcome to use the Content Information Type Specifications to achieve interoperability at a more detailed level.</p>

<p>The core metadata requirements are described using METS (Metadata Encoding &amp; Transmission Standard, <a href="http://www.loc.gov/standards/mets/">http://www.loc.gov/standards/mets/</a>). We describe the core elements used, METS describes other available elements which may be used in addition to those detailed in the CSIP.</p>

<p>Some metadata requirements are implied by the structure presented in the previous section. As seen, one or more METS files can be present in a package. The METS file describing the whole package is from now called the “Package METS”, and the METS file in the representation folders are called “Representation METS”. The detailed specification of using METS within the CSIP is available in Section 5.3.</p>

<p>In addition to the METS files, the CSIP recommends the inclusion of PREMIS metadata (PREservation Metadata Implementation Strategies, <a href="http://www.loc.gov/standards/premis/">http://www.loc.gov/standards/premis/</a>), placed in appropriate preservation metadata folders. This facilitates interoperable approach towards provenance and access to Information Packages. However, it is recognised that, especially in the case of SIPs, appropriate preservation metadata is not always available. As such, this is also not an absolute requirement though highly desirable. A specification of the use of PREMIS within the CSIP is available in Section 5.4.</p>

<p>The specification does not prohibit the use of additional metadata within Information Packages.</p>

<p><a name="generalrequirementsfortheuseofmetadata"></a></p>

<h2 id="52-general-requirements-for-the-use-of-metadata">5.2. General requirements for the use of metadata</h2>
<p>Before detailing the requirements covering the use of METS and PREMIS, it is necessary to highlight some general metadata concerns which should be handled consistently.</p>

<p><a name="theuseofidentifiers"></a></p>

<h3 id="521-the-use-of-identifiers">5.2.1. The use of identifiers</h3>
<p>Both METS, and by derivation the CSIP, make extensive use of the XML ID data type (see: <a href="https://www.w3.org/TR/xml-id/">https://www.w3.org/TR/xml-id/</a>). Valid XML IDs must also conform to the NCName restrictions (see: <a href="https://www.w3.org/TR/REC-xml-names/#NT-NCName">https://www.w3.org/TR/REC-xml-names/#NT-NCName</a>), and must begin a letter or an underscore character (‘_’), and contain no characters other than letters, digits, hyphens, underscores, full stops, plus some extension and combination characters.</p>

<p>If a package makes use of IDs that do not conform to this specification, one mitigating strategy is to add a prefix to all identifiers. For example, UUIDs are a common choice for arbitrary identifiers and comprise of hex characters and hyphens (e.g. the value <code class="language-plaintext highlighter-rouge">906F4F12-BA52-4779-AE2C-178F9206111F</code>). NCName and xml:id values cannot legally begin with numeric characters making many UUIDs, including the example, invalid. The examples below show two possible solutions, using prefixes:</p>

<p>Example 1: The prefix consists of the identifier type acronym and a hyphen: <code class="language-plaintext highlighter-rouge">uuid-</code>.</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;dmdSec</span> <span class="na">ID=</span><span class="s">"uuid-906F4F12-BA52-4779-AE2C-178F9206111F"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.609+01:00"</span><span class="nt">&gt;</span>
</code></pre></div></div>

<p>Example 2: A generic prefix:<code class="language-plaintext highlighter-rouge">ID</code>.</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;dmdSec</span> <span class="na">ID=</span><span class="s">"ID906F4F12-BA52-4779-AE2C-178F9206111F"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.609+01:00"</span><span class="nt">&gt;</span>
</code></pre></div></div>

<p>The identifiers specified within the CSIP are mainly used as internal references between Information Package components. Prefixes are not mandatory, but if they are used, it is recommended that a single prefix is chosen and used consistently across all IDs in the package.</p>

<p>Note that while we recommend the use of generated unique IDs in real world information packages we used logical unique names for the examples in this document. This is for readability purposes, particularly for any readers trying to follow reference links.</p>

<p><a name="referencingbetweenfileswithinacsipinformationpackage"></a></p>

<h3 id="522-referencing-between-files-within-a-csip-information-package">5.2.2. Referencing between files within a CSIP Information Package</h3>
<p>It is strongly recommended that all components of an information package (i.e. all data, metadata and other parts) are stored as discrete files within the package. While this approach simplifies the management of the Information Package, making it easier to aggregate, validate and modify the package, it also necessitates a clear method for recording and resolving referencing between files.</p>

<p>For example, when using the CSIP referencing can occur between:</p>

<ul>
  <li>descriptive and administrative metadata files described in the <code class="language-plaintext highlighter-rouge">amdSec</code> and <code class="language-plaintext highlighter-rouge">dmdSec</code> elements;</li>
  <li>content (data) files, components of documentation, and schemas described in the <code class="language-plaintext highlighter-rouge">fileSec</code> element;</li>
  <li>representation METS files described in the Package METS file’s <code class="language-plaintext highlighter-rouge">fileSec</code> and <code class="language-plaintext highlighter-rouge">structMap</code> elements.</li>
</ul>

<p>A consistent approach to referencing between package components is a fundamental requirement for Information Package validation and integrity checking. Different technical solutions exist for referencing and resolving, but they are not universally supported by all digital preservation tools. To ensure interoperability, all references within a CSIP Information Package must adhere to the requirements stated in this specification.</p>

<p><a name="referencingotherpackages"></a></p>

<h3 id="523-referencing-other-packages">5.2.3. Referencing other packages</h3>
<p>It is important that external references (i.e. to other packages) are expressed consistently, in the same manner as internal references. All references to other packages MUST USE the <code class="language-plaintext highlighter-rouge">mets/@OBJID</code> value of the target package.</p>

<p><a name="examples"></a></p>

<h3 id="524-examples">5.2.4. Examples</h3>
<p>This document illustrates the use of the specification with generic examples. These examples use values from vocabularies and elements defined by the CSIP to demonstrate some specific uses of the specification. Outside these CSIP specific values, the METS values are fictive and are not meant to constitute real-life examples. More complete examples will be provided in the CSIP user guidelines that will be published at a future date.</p>

<p><a name="useofmets"></a></p>

<h2 id="53-use-of-mets">5.3. Use of METS</h2>
<p>The main requirement for METS files in a CSIP Information Package is that these need to follow the official METS Schema version 1.12 <a href="http://www.loc.gov/standards/mets/mets-schemadocs.html">http://www.loc.gov/standards/mets/mets-schemadocs.html</a> (by CSIP used version in May 2019) and the extension schema developed for the CSIP and published by the DILCIS Board. As new versions of METS Schema become available the DILCIS Board will evaluate these and, if necessary, update the CSIP respectively.</p>

<p>The following text assumes knowledge of the principles of the METS specification. If this is not the case, please consult the official documentation before continuing.</p>

<p>The METS specification requires a METS profile document which describes the use of METS and the METS elements. All the requirements described in this specification is also expressed with a METS profile for the CSIP <a href="https://github.com/DILCISBoard/E-ARK-CSIP/tree/master/profile">https://github.com/DILCISBoard/E-ARK-CSIP/tree/master/profile</a>.</p>

<p>METS allows metadata to be both embedded and referenced. The CSIP itself allows both the embedding of metadata within the <code class="language-plaintext highlighter-rouge">METS.xml</code> file but note that for scalability concerns the CSIP only recommends the use of referencing. This means that the CSIP only describes referencing of metadata.</p>

<p>The rest of this section describes the use of each of the METS elements: mets, metsHdr, dmdSec, amdSec, fileSec and structMap. For each element, the restrictions imposed by the CSIP on top or those in the official METS documentation are explained. A CSIP implementation can choose to extend the restrictions in line with requirements specific to the implementation. In these cases follow the METS documentation and create an implementation which uses the CSIP as a base profile.</p>

<p>Differences between creating a package METS file and representation METS file are described when relevant.</p>

<p>All names of elements and attributes below are expressed using the XPath notation (i.e. <code class="language-plaintext highlighter-rouge">element/sub-element/@attribute</code>)</p>

<p><a name="useofthemetsrootelementelementmets"></a></p>

<h3 id="531-use-of-the-mets-root-element-element-mets">5.3.1. Use of the METS root element (element mets)</h3>
<p>The METS document’s root element (<code class="language-plaintext highlighter-rouge">&lt;mets&gt;</code>) describes the container for the information being stored and/or transmitted. The <code class="language-plaintext highlighter-rouge">&lt;mets&gt;</code> element of a CSIP conformant METS document uses attributes from the METS specification and additional attributes defined in the CSIP extension schema.</p>

<p>As well as the METS and CSIP extension attributes, the METS document’s root <code class="language-plaintext highlighter-rouge">&lt;mets&gt;</code> element must define all of the relevant namespaces and locations for XML schema used in the package. This is done using the <code class="language-plaintext highlighter-rouge">@xmlns</code> and <code class="language-plaintext highlighter-rouge">@xsi:schemaLocation</code> attributes as described in <a href="https://www.w3schools.com/xml/schema_schema.asp">“Referencing a Schema in an XML Document”</a>. The schema identifiers and locations for a typical CSIP <code class="language-plaintext highlighter-rouge">&lt;mets&gt;</code> element are shown below:</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code>  <span class="nt">&lt;mets:mets</span> <span class="na">xmlns:xsi=</span><span class="s">"http://www.w3.org/2001/XMLSchema-instance"</span>
    <span class="na">xmlns:mets=</span><span class="s">"http://www.loc.gov/METS/"</span>
    <span class="na">xmlns:xlink=</span><span class="s">"http://www.w3.org/1999/xlink"</span>
    <span class="na">xmlns:csip=</span><span class="s">"https://dilcis.eu/XML/METS/CSIPExtensionMETS"</span>
    <span class="na">xsi:schemaLocation=</span><span class="s">"http://www.loc.gov/METS/ http://www.loc.gov/standards/mets/mets.xsd
                       http://www.w3.org/1999/xlink http://www.loc.gov/standards/mets/xlink.xsd
                       https://dilcis.eu/XML/METS/CSIPExtensionMETS https://earkcsip.dilcis.eu/schema/DILCISExtensionMETS.xsd"</span><span class="nt">&gt;</span>
</code></pre></div></div>
<p><a name="locationofxmlschema"></a></p>

<h4 id="5311-location-of-xml-schema">5.3.1.1. Location of XML schema</h4>
<p>When using XML schemas the availability of the actual schema resources should be considered. Externally hosted resources are not guaranteed to be available in the future, or in restricted operating environments. We recommend that copies of all XML schema resources should be included in the information package, located in appropriate ‘schemas’ folders at package or representation level. When schemas have been included in the package <code class="language-plaintext highlighter-rouge">schemas</code> folder, links to the schema documents should refer to the relative path of the schema file within the package, i.e. <code class="language-plaintext highlighter-rouge">schemas/mets.xsd</code>.</p>

<p>The specific requirements for the root element and its attributes are described in the following table.</p>

<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Name, Location &amp; Description</th>
      <th>Card &amp; Level</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
<a name="CSIP1"></a><strong>CSIP1</strong>
</td>
      <td>
<strong>Package Identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/@OBJID</code> <br> The <code class="language-plaintext highlighter-rouge">mets/@OBJID</code> attribute is mandatory, its value is a string identifier for the METS document. For the package METS document, this should be the name/ID of the package, i.e. the name of the package root folder. <br> For a representation level METS document this value records the name/ID of the representation, i.e. the name of the top-level representation folder.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP2"></a><strong>CSIP2</strong>
</td>
      <td>
<strong>Content Category</strong> <br> <code class="language-plaintext highlighter-rouge">mets/@TYPE</code> <br> The <code class="language-plaintext highlighter-rouge">mets/@TYPE</code> attribute MUST be used to declare the category of the content held in the package, e.g. book, journal, stereograph, video, etc.. Legal values are defined in a fixed vocabulary. When the content category used falls outside of the defined vocabulary the <code class="language-plaintext highlighter-rouge">mets/@TYPE</code> value must be set to “OTHER” and the specific value declared in <code class="language-plaintext highlighter-rouge">mets/@csip:OTHERTYPE</code>. The vocabulary will develop under the curation of the DILCIS Board as additional content information type specifications are produced. <br> <strong>See also:</strong> <a href="#VocabularyContentCategory">Content Category</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP3"></a><strong>CSIP3</strong>
</td>
      <td>
<strong>Other Content Category</strong> <br> <code class="language-plaintext highlighter-rouge">mets[@TYPE='OTHER']/@csip:OTHERTYPE</code> <br> When the <code class="language-plaintext highlighter-rouge">mets/@TYPE</code> attribute has the value “OTHER” the <code class="language-plaintext highlighter-rouge">mets/@csip:OTHERTYPE</code> attribute MUST be used to declare the content category of the package/representation. <br> <strong>See also:</strong> <a href="#VocabularyContentCategory">Content Category</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP4"></a><strong>CSIP4</strong>
</td>
      <td>
<strong>Content Information Type Specification</strong> <br> <code class="language-plaintext highlighter-rouge">mets/@csip:CONTENTINFORMATIONTYPE</code> <br> Used to declare the Content Information Type Specification used when creating the package. Legal values are defined in a fixed vocabulary. The attribute is mandatory for representation level METS documents. The vocabulary will evolve under the care of the DILCIS Board as additional Content Information Type Specifications are developed. <br> <strong>See also:</strong> <a href="#VocabularyContentInformationTypeSpecification">Content information type specification</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP5"></a><strong>CSIP5</strong>
</td>
      <td>
<strong>Other Content Information Type Specification</strong> <br> <code class="language-plaintext highlighter-rouge">mets[@csip:CONTENTINFORMATIONTYPE='OTHER']/@csip:OTHERCONTENTINFORMATIONTYPE</code> <br> When the <code class="language-plaintext highlighter-rouge">mets/@csip:CONTENTINFORMATIONTYPE</code> has the value “OTHER” the <code class="language-plaintext highlighter-rouge">mets/@csip:OTHERCONTENTINFORMATIONTYPE</code> must state the content information type.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP6"></a><strong>CSIP6</strong>
</td>
      <td>
<strong>METS Profile</strong> <br> <code class="language-plaintext highlighter-rouge">mets/@PROFILE</code> <br> The URL of the METS profile that the information package conforms with.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
  </tbody>
</table>

<p><strong>Example:</strong> METS root element showing use of <code class="language-plaintext highlighter-rouge">csip:@OTHERTYPE</code> attribute when an appropriate package content category value is not available in the vocabulary. The <code class="language-plaintext highlighter-rouge">@TYPE</code> attribute value is set to OTHER.</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:mets</span> <span class="na">xmlns:csip=</span><span class="s">"https://DILCIS.eu/XML/METS/CSIPExtensionMETS"</span> <span class="na">xmlns:mets=</span><span class="s">"http://www.loc.gov/METS/"</span> <span class="na">xmlns:xsi=</span><span class="s">"http://www.w3.org/2001/XMLSchema-instance"</span> <span class="na">xmlns:xlink=</span><span class="s">"http://www.w3.org/1999/xlink"</span> <span class="na">OBJID=</span><span class="s">"csip-mets-example"</span> <span class="na">LABEL=</span><span class="s">"Sample CSIP Information Package"</span> <span class="na">TYPE=</span><span class="s">"OTHER"</span> <span class="na">csip:OTHERTYPE=</span><span class="s">"Patterns"</span> <span class="na">PROFILE=</span><span class="s">"https://earkcsip.dilcis.eu/profile/E-ARK-CSIP.xml"</span> <span class="na">xsi:schemaLocation=</span><span class="s">"http://www.loc.gov/METS/ http://www.loc.gov/standards/mets/mets.xsd http://www.w3.org/1999/xlink http://www.loc.gov/standards/mets/xlink.xsd https://DILCIS.eu/XML/METS/CSIPExtensionMETS https://earkcsip.dilcis.eu/schema/DILCISExtensionMETS.xsd"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/mets:mets&gt;</span>
</code></pre></div></div>

<p><strong>Example:</strong> METS root element illustrating the use of a custom <code class="language-plaintext highlighter-rouge">csip:@OTHERCONTENTINFORMATIONTYPE</code> attribute value when the correct content type value does note exist in the vocabulary. The <code class="language-plaintext highlighter-rouge">csip:@CONTENTINFORMATIONTYPE</code> attribute value is set to OTHER.</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:mets</span> <span class="na">xmlns:csip=</span><span class="s">"https://DILCIS.eu/XML/METS/CSIPExtensionMETS"</span> <span class="na">xmlns:mets=</span><span class="s">"http://www.loc.gov/METS/"</span> <span class="na">xmlns:xsi=</span><span class="s">"http://www.w3.org/2001/XMLSchema-instance"</span> <span class="na">xmlns:xlink=</span><span class="s">"http://www.w3.org/1999/xlink"</span> <span class="na">OBJID=</span><span class="s">"csip-mets-example"</span> <span class="na">LABEL=</span><span class="s">"Sample CSIP Information Package"</span> <span class="na">TYPE=</span><span class="s">"Datasets"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"OTHER"</span> <span class="na">csip:OTHERCONTENTINFORMATIONTYPE=</span><span class="s">"FGS Personal, version 1"</span> <span class="na">PROFILE=</span><span class="s">"https://earkcsip.dilcis.eu/profile/E-ARK-CSIP.xml"</span> <span class="na">xsi:schemaLocation=</span><span class="s">"http://www.loc.gov/METS/ http://www.loc.gov/standards/mets/mets.xsd http://www.w3.org/1999/xlink http://www.loc.gov/standards/mets/xlink.xsd https://DILCIS.eu/XML/METS/CSIPExtensionMETS https://earkcsip.dilcis.eu/schema/DILCISExtensionMETS.xsd"</span><span class="nt">&gt;</span>
<span class="nt">&lt;/mets:mets&gt;</span>
</code></pre></div></div>

<p><a name="useofthemetsheaderelementmetshdr"></a></p>

<h3 id="532-use-of-the-mets-header-element-metshdr">5.3.2. Use of the METS header (element metsHdr)</h3>
<p>The purpose of the METS header section is to describe the METS document itself, for example information
about the creator of the IP. The requirements for the metsHdr element, its sub-elements and attributes are presented in the following
table.</p>

<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Name, Location &amp; Description</th>
      <th>Card &amp; Level</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
<a name="CSIP117"></a><strong>CSIP117</strong>
</td>
      <td>
<strong>Package header</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr</code> <br> General element for describing the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP7"></a><strong>CSIP7</strong>
</td>
      <td>
<strong>Package creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@CREATEDATE</code> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@CREATEDATE</code> records the date the package was created.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP8"></a><strong>CSIP8</strong>
</td>
      <td>
<strong>Package last modification date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@LASTMODDATE</code> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@LASTMODDATE</code> is mandatory when the package has been modified.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP9"></a><strong>CSIP9</strong>
</td>
      <td>
<strong>OAIS Package type information</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@csip:OAISPACKAGETYPE</code> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@csip:OAISPACKAGETYPE</code> is an additional CSIP attribute that declares the type of the IP. <br> <strong>See also:</strong> <a href="#VocabularyOAISPackageType">OAIS Package type</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP10"></a><strong>CSIP10</strong>
</td>
      <td>
<strong>Agent</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent</code> <br> A mandatory agent element records the software used to create the package. Other uses of agents may be described in any local implementations that extend the profile.</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP11"></a><strong>CSIP11</strong>
</td>
      <td>
<strong>Agent role</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent[@ROLE='CREATOR']</code> <br> The mandatory agent element MUST have a <code class="language-plaintext highlighter-rouge">@ROLE</code> attribute with the value “CREATOR”.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP12"></a><strong>CSIP12</strong>
</td>
      <td>
<strong>Agent type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent[@TYPE='OTHER']</code> <br> The mandatory agent element MUST have a <code class="language-plaintext highlighter-rouge">@TYPE</code> attribute with the value “OTHER”.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP13"></a><strong>CSIP13</strong>
</td>
      <td>
<strong>Agent other type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent[@OTHERTYPE='SOFTWARE']</code> <br> The mandatory agent element MUST have a <code class="language-plaintext highlighter-rouge">@OTHERTYPE</code> attribute with the value “SOFTWARE”. <br> <strong>See also:</strong> <a href="#VocabularyAgentOtherType">Other agent type</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP14"></a><strong>CSIP14</strong>
</td>
      <td>
<strong>Agent name</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent/name</code> <br> The mandatory agent’s name element records the name of the software tool used to create the IP.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP15"></a><strong>CSIP15</strong>
</td>
      <td>
<strong>Agent additional information</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent/note</code> <br> The mandatory agent’s note element records the version of the tool used to create the IP.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP16"></a><strong>CSIP16</strong>
</td>
      <td>
<strong>Classification of the agent additional information</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent/note[@csip:NOTETYPE='SOFTWARE VERSION']</code> <br> The mandatory agent element’s note child has a <code class="language-plaintext highlighter-rouge">@csip:NOTETYPE</code> attribute with a fixed value of “SOFTWARE VERSION”. <br> <strong>See also:</strong> <a href="#VocabularyNoteType">Note type</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
  </tbody>
</table>

<p><strong>Example:</strong> METS agent example of the mandatory agent</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:metsHdr</span> <span class="na">CREATEDATE=</span><span class="s">"2018-04-24T14:37:49.602+01:00"</span> <span class="na">LASTMODDATE=</span><span class="s">"2018-04-24T14:37:49.602+01:00"</span> <span class="na">RECORDSTATUS=</span><span class="s">"NEW"</span> <span class="na">csip:OAISPACKAGETYPE=</span><span class="s">"SIP"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;mets:agent</span> <span class="na">ROLE=</span><span class="s">"CREATOR"</span> <span class="na">TYPE=</span><span class="s">"OTHER"</span> <span class="na">OTHERTYPE=</span><span class="s">"SOFTWARE"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:name&gt;</span>RODA-in<span class="nt">&lt;/mets:name&gt;</span>
    <span class="nt">&lt;mets:note</span> <span class="na">csip:NOTETYPE=</span><span class="s">"SOFTWARE VERSION"</span><span class="nt">&gt;</span>2.1.0-beta.7<span class="nt">&lt;/mets:note&gt;</span>
  <span class="nt">&lt;/mets:agent&gt;</span>
<span class="nt">&lt;/mets:metsHdr&gt;</span>
</code></pre></div></div>

<p><a name="useofthemetsdescriptivemetadatasectionelementdmdsec"></a></p>

<h3 id="533-use-of-the-mets-descriptive-metadata-section-element-dmdsec">5.3.3. Use of the METS descriptive metadata section (element dmdSec)</h3>

<p>The purpose of the METS descriptive metadata section is to embed or refer to files containing descriptive metadata. CSIP is only using referencing of files containing descriptive metadata.</p>

<p>The CSIP does not prescribe or assume the use of specific descriptive metadata schemas. This means implementers are free to use descriptive metadata  standards of their choosing inside a CSIP package.</p>

<p>Specific elements for which the exact use is fixed within this specification are highlighted in the following table.</p>

<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Name, Location &amp; Description</th>
      <th>Card &amp; Level</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
<a name="CSIP17"></a><strong>CSIP17</strong>
</td>
      <td>
<strong>Descriptive metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec</code> <br> Must be used if descriptive metadata for the package content is available. Each descriptive metadata section (<code class="language-plaintext highlighter-rouge">&lt;dmdSec&gt;</code>) contains a single description and must be repeated for multiple descriptions, when available. <br> It is possible to transfer metadata in a package using just the descriptive metadata section and/or administrative metadata section.</td>
      <td>
<strong>0..n</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP18"></a><strong>CSIP18</strong>
</td>
      <td>
<strong>Descriptive metadata identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the descriptive metadata section (<code class="language-plaintext highlighter-rouge">&lt;dmdSec&gt;</code>) used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP19"></a><strong>CSIP19</strong>
</td>
      <td>
<strong>Descriptive metadata creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/@CREATED</code> <br> Creation date of the descriptive metadata in this section.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP20"></a><strong>CSIP20</strong>
</td>
      <td>
<strong>Status of the descriptive metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/@STATUS</code> <br> Indicates the status of the package using a fixed vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStatus">dmdSec status</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP21"></a><strong>CSIP21</strong>
</td>
      <td>
<strong>Reference to the document with the descriptive metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef</code> <br> Reference to the descriptive metadata file located in the “metadata” section of the IP.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP22"></a><strong>CSIP22</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP23"></a><strong>CSIP23</strong>
</td>
      <td>
<strong>Type of link</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP24"></a><strong>CSIP24</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@xlink:href</code> <br> The actual location of the resource. This specification recommends recording a URL type filepath in this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP25"></a><strong>CSIP25</strong>
</td>
      <td>
<strong>Type of metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@MDTYPE</code> <br> Specifies the type of metadata in the referenced file. Values are taken from the list provided by the METS.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP26"></a><strong>CSIP26</strong>
</td>
      <td>
<strong>File mime type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@MIMETYPE</code> <br> The IANA mime type of the referenced file. <br> <strong>See also:</strong> <a href="#VocabularyIANAmediaTypes">IANA media types</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP27"></a><strong>CSIP27</strong>
</td>
      <td>
<strong>File size</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@SIZE</code> <br> Size of the referenced file in bytes.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP28"></a><strong>CSIP28</strong>
</td>
      <td>
<strong>File creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@CREATED</code> <br> The creation date of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP29"></a><strong>CSIP29</strong>
</td>
      <td>
<strong>File checksum</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@CHECKSUM</code> <br> The checksum of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP30"></a><strong>CSIP30</strong>
</td>
      <td>
<strong>File checksum type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@CHECKSUMTYPE</code> <br> The type of checksum following the value list present in the METS-standard which has been used for calculating the checksum for the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
  </tbody>
</table>

<p><strong>Example:</strong> METS example of referencing the descriptive metadata which is described with an EAD document</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:dmdSec</span> <span class="na">ID=</span><span class="s">"dmd-ead-file"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.609+01:00"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">MDTYPE=</span><span class="s">"EAD"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/descriptive/ead2002.xml"</span> <span class="na">MIMETYPE=</span><span class="s">"application/xml"</span> <span class="na">SIZE=</span><span class="s">"903"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.609+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"F24263BF09994749F335E1664DCE0086DB6DCA323FDB6996938BCD28EA9E8153"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;/mets:mdRef&gt;</span>
<span class="nt">&lt;/mets:dmdSec&gt;</span>
</code></pre></div></div>

<p><a name="useofthemetsadministrativemetadatasectionelementamdsec"></a></p>

<h3 id="534-use-of-the-mets-administrative-metadata-section-element-amdsec">5.3.4. Use of the METS administrative metadata section (element amdSec)</h3>
<p>METS defines an administrative metadata section, used to embed metadata or provide references to files containing metadata for the information package content. The CSIP encourages the use of references to metadata files, rather than embedding metadata in the <code class="language-plaintext highlighter-rouge">amdSec</code> element, and the examples reflect this.</p>

<p>The administrative metadata section contains four sub-sections each used to record different types of metadata for package content:</p>
<ul>
  <li>technical metadata (element techMD) records technical metadata;</li>
  <li>rights metadata (element rightsMD) records intellectual property rights information;</li>
  <li>source metadata (element sourceMD) records descriptive, technical or rights metadata for an analog source for a digital library object; and</li>
  <li>digital provenance metadata (element digiprovMD) records digital preservation information, e.g. audit information covering a digital library object’s life-cycle.</li>
</ul>

<p>The CSIP only describes use of the elements <code class="language-plaintext highlighter-rouge">digiprovMD</code> and <code class="language-plaintext highlighter-rouge">rightsMD</code>. The population of the other metadata sections are left to local policy and practise.</p>

<p>The CSIP (and METS) categorises preservation metadata as administrative metadata, specifically Digital Provenance metadata (following the avaiable guidelines published by the PREMIS EC guidelines: <a href="http://www.loc.gov/standards/premis/guidelines2017-premismets.pdf">http://www.loc.gov/standards/premis/guidelines2017-premismets.pdf</a>), hence all preservation metadata should be referenced from a <code class="language-plaintext highlighter-rouge">digiprovMD</code> element within the <code class="language-plaintext highlighter-rouge">amdSec</code>.</p>

<p>The METS <code class="language-plaintext highlighter-rouge">amdSec</code> element SHOULD include references to all relevant metadata located in the folder “metadata/preservation”. The package level <code class="language-plaintext highlighter-rouge">METS.xml</code> file SHOULD only reference package level preservation metadata. Representation level <code class="language-plaintext highlighter-rouge">METS.xml</code> files SHOULD only reference representation level preservation metadata.</p>

<p>The specific requirements for the <code class="language-plaintext highlighter-rouge">amdSec</code> element, its sub-elements and attributes are presented in the following table.</p>

<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Name, Location &amp; Description</th>
      <th>Card &amp; Level</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
<a name="CSIP31"></a><strong>CSIP31</strong>
</td>
      <td>
<strong>Administrative metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec</code> <br> If administrative / preservation metadata is available, it must be described using the administrative metadata section (<code class="language-plaintext highlighter-rouge">&lt;amdSec&gt;</code>) element. <br> All administrative metadata is present in a single <code class="language-plaintext highlighter-rouge">&lt;amdSec&gt;</code> element. <br> It is possible to transfer metadata in a package using just the descriptive metadata section and/or administrative metadata section.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP32"></a><strong>CSIP32</strong>
</td>
      <td>
<strong>Digital provenance metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD</code> <br> For recording information about preservation the standard PREMIS is used. It is mandatory to include one <code class="language-plaintext highlighter-rouge">&lt;digiprovMD&gt;</code> element for each piece of PREMIS metadata. <br> The use if PREMIS in METS is following the recommendations in  <a href="http://www.loc.gov/standards/premis/guidelines2017-premismets.pdf"> the 2017 version of PREMIS in METS Guidelines.</a>
</td>
      <td>
<strong>0..n</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP33"></a><strong>CSIP33</strong>
</td>
      <td>
<strong>Digital provenance metadata identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the digital provenance metadata section <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD</code> used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP34"></a><strong>CSIP34</strong>
</td>
      <td>
<strong>Status of the digital provenance metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/@STATUS</code> <br> Indicates the status of the package using a fixed vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStatus">dmdSec status</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP35"></a><strong>CSIP35</strong>
</td>
      <td>
<strong>Reference to the document with the digital provenance metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef</code> <br> Reference to the digital provenance metadata file stored in the “metadata” section of the IP.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP36"></a><strong>CSIP36</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP37"></a><strong>CSIP37</strong>
</td>
      <td>
<strong>Type of link</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP38"></a><strong>CSIP38</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@xlink:href</code> <br> The actual location of the resource. This specification recommends recording a URL type filepath within this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP39"></a><strong>CSIP39</strong>
</td>
      <td>
<strong>Type of metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@MDTYPE</code> <br> Specifies the type of metadata in the referenced file. Values are taken from the list provided by the METS.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP40"></a><strong>CSIP40</strong>
</td>
      <td>
<strong>File mime type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@MIMETYPE</code> <br> The IANA mime type for the referenced file. <br> <strong>See also:</strong> <a href="#VocabularyIANAmediaTypes">IANA media types</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP41"></a><strong>CSIP41</strong>
</td>
      <td>
<strong>File size</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@SIZE</code> <br> Size of the referenced file in bytes.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP42"></a><strong>CSIP42</strong>
</td>
      <td>
<strong>File creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@CREATED</code> <br> Creation date of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP43"></a><strong>CSIP43</strong>
</td>
      <td>
<strong>File checksum</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@CHECKSUM</code> <br> The checksum of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP44"></a><strong>CSIP44</strong>
</td>
      <td>
<strong>File checksum type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@CHECKSUMTYPE</code> <br> The type of checksum following the value list present in the METS-standard which has been used for calculating the checksum for the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP45"></a><strong>CSIP45</strong>
</td>
      <td>
<strong>Rights metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD</code> <br> A simple rights statement may be used to describe general permissions for the package. Individual representations should state their specific rights in their representation METS file. <br> Available standards include  <a href="http://rightsstatements.org">RightsStatements.org</a> ,  <a href="https://pro.europeana.eu/page/available-rights-statements">Europeana rights statements info</a> ,  <a href="https://github.com/mets/METS-Rights-Schema">METS Rights Schema</a>  created and maintained by the METS Board, the rights part of  <a href="http://www.loc.gov/standards/premis/">PREMIS</a>  as well as own local rights statements in use.</td>
      <td>
<strong>0..n</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP46"></a><strong>CSIP46</strong>
</td>
      <td>
<strong>Rights metadata identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the rights metadata section (<code class="language-plaintext highlighter-rouge">&lt;rightsMD&gt;</code>) used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP47"></a><strong>CSIP47</strong>
</td>
      <td>
<strong>Status of the rights metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/@STATUS</code> <br> Indicates the status of the package using a fixed vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStatus">dmdSec status</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP48"></a><strong>CSIP48</strong>
</td>
      <td>
<strong>Reference to the document with the rights metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef</code> <br> Reference to the rights metadata file stored in the “metadata” section of the IP.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP49"></a><strong>CSIP49</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP50"></a><strong>CSIP50</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP51"></a><strong>CSIP51</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@xlink:href</code> <br> The actual location of the resource. We  recommend recording a URL type filepath within this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP52"></a><strong>CSIP52</strong>
</td>
      <td>
<strong>Type of metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@MDTYPE</code> <br> Specifies the type of metadata in the referenced file. Value is taken from the list provided by the METS.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP53"></a><strong>CSIP53</strong>
</td>
      <td>
<strong>File mime type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@MIMETYPE</code> <br> The IANA mime type for the referenced file. <br> <strong>See also:</strong> <a href="#VocabularyIANAmediaTypes">IANA media types</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP54"></a><strong>CSIP54</strong>
</td>
      <td>
<strong>File size</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@SIZE</code> <br> Size of the referenced file in bytes.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP55"></a><strong>CSIP55</strong>
</td>
      <td>
<strong>File creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@CREATED</code> <br> Creation date of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP56"></a><strong>CSIP56</strong>
</td>
      <td>
<strong>File checksum</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@CHECKSUM</code> <br> The checksum of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP57"></a><strong>CSIP57</strong>
</td>
      <td>
<strong>File checksum type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@CHECKSUMTYPE</code> <br> The type of checksum following the value list present in the METS-standard which has been used for calculating the checksum for the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
  </tbody>
</table>

<p><strong>Example:</strong> METS example of referencing preservation metadata in the form of PREMIS metadata for describing the preservation objects and the events pertaining to the objects</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:amdSec&gt;</span>
  <span class="nt">&lt;mets:digiprovMD</span> <span class="na">ID=</span><span class="s">"digiprov-premis-file-1"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/preservation/premis1.xml"</span> <span class="na">MDTYPE=</span><span class="s">"PREMIS"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"3.0"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xml"</span> <span class="na">SIZE=</span><span class="s">"1211"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"8aa278038dbad54bbf142e7d72b493e2598a94946ea1304dc82a79c6b4bac3d5"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">LABEL=</span><span class="s">"premis1.xml"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;/mets:mdRef&gt;</span>
  <span class="nt">&lt;/mets:digiprovMD&gt;</span>
  <span class="nt">&lt;mets:digiprovMD</span> <span class="na">ID=</span><span class="s">"digiprov-premis-file-2"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:47:52.783+01:00"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/preservation/premis2.xml"</span> <span class="na">MDTYPE=</span><span class="s">"PREMIS"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"3.0"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xml"</span> <span class="na">SIZE=</span><span class="s">"2854"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"d1dfa585dcc9d87268069dc58d5e47956434ec3db4087a75a3885d287f15126f"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">LABEL=</span><span class="s">"premis2.xml"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;/mets:mdRef&gt;</span>
  <span class="nt">&lt;/mets:digiprovMD&gt;</span>
<span class="nt">&lt;/mets:amdSec&gt;</span>
</code></pre></div></div>

<p><a name="useofthemetsfilesectionelementfilesec"></a></p>

<h3 id="535-use-of-the-mets-file-section-element-filesec">5.3.5. Use of the METS file section (element fileSec)</h3>
<p>The CSIP does not make the use of the METS fileSec element mandatory, but it is strongly recommended. The fileSec should describe every component of the IP not already described in the amdSec and dmdSec elements. Location and checksum values must be provided for all file entries.</p>

<p>The METS file section serves as a manifest, allowing users to ensure all files are present and that a package is complete, as well as testing the integrity of package files using checksum values.</p>

<p>The files are described in a file group element named <code class="language-plaintext highlighter-rouge">fileGrp</code>. The <code class="language-plaintext highlighter-rouge">fileGrp</code> element contains the descriptions of the files including their checksum and location. It is possible to nest <code class="language-plaintext highlighter-rouge">fileGrp</code> elements within other <code class="language-plaintext highlighter-rouge">fileGrp</code> elements, however the CSIP states that hierarchical nesting SHOULD NOT be used.</p>

<p>The CSIP requires that both package and representation level METS files include at least three file group (fileGrp) elements. The CSIP divides the referenced files into categories, i.e. documentation. schemas, data, each contained within its own fileGrp element. It is possible to add own additional file groups following the same file groups requirements described in CSIP. Representation level METS files should not reference files outside of their representation. That is they should not contain references to package level files or files from other representations. The package level METS file should contain a fileGrp element for each representation which contains a single reference to the representation’s METS.xml file. This is to ensure that the package lists all representations and their locations for completeness and integrity checks.</p>

<p>The specific requirements for elements, sub-elements and attributes are listed in the following table. Note that the use of the stream and transformFile elements is not discussed below. Implementers wishing to use either of these METS elements should follow the requirements in the METS documentation.</p>

<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Name, Location &amp; Description</th>
      <th>Card &amp; Level</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
<a name="CSIP58"></a><strong>CSIP58</strong>
</td>
      <td>
<strong>File section</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec</code> <br> The transferred content is placed in the file section in different file group elements, described in other requirements. <br> Only a single file section (<code class="language-plaintext highlighter-rouge">&lt;fileSec&gt;</code>) element should be present. <br> It is possible to transfer just descriptive metadata and/or administrative metadata without files placed in this section.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP59"></a><strong>CSIP59</strong>
</td>
      <td>
<strong>File section identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the file section used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP60"></a><strong>CSIP60</strong>
</td>
      <td>
<strong>Documentation file group</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@USE='Documentation']</code> <br> All documentation pertaining to the transferred content is placed in one or more file group elements with <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> attribute value “Documentation”. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP113"></a><strong>CSIP113</strong>
</td>
      <td>
<strong>Schema file group</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@USE='Schemas']</code> <br> All XML schemas used in the information package should be referenced from one or more file groups with <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> attribute value “Schemas”. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP114"></a><strong>CSIP114</strong>
</td>
      <td>
<strong>Representations file group</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@USE='Representations']</code> <br> A pointer to the METS document describing the representation or pointers to the content being transferred must be present in one or more file groups with <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> attribute value “Representations”. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP61"></a><strong>CSIP61</strong>
</td>
      <td>
<strong>Reference to administrative metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@ADMID</code> <br> If administrative metadata has been provided at file group  <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp</code> level this attribute refers to its administrative metadata section by ID.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP62"></a><strong>CSIP62</strong>
</td>
      <td>
<strong>Content Information Type Specification</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@USE='Representations']/@csip:CONTENTINFORMATIONTYPE</code> <br> An added attribute which states the name of the content information type specification used to create the package. <br> The vocabulary will evolve under the curation of the DILCIS Board as additional content information type specifications are developed. <br> This attribute is mandatory when the <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> attribute value is “Representations”. <br> When the “Package type” value is “Mixed” and/or the file group describes a “Representation”, then this element states the content information type specification used for the file group. <br> <strong>See also:</strong> <a href="#VocabularyContentInformationTypeSpecification">Content information type specification</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP63"></a><strong>CSIP63</strong>
</td>
      <td>
<strong>Other Content Information Type Specification</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@csip:CONTENTINFORMATIONTYPE='OTHER']/@csip:OTHERCONTENTINFORMATIONTYPE</code> <br> When the <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@csip:CONTENTINFORMATIONTYPE</code> attribute has the value “OTHER” the <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@csip:OTHERCONTENTINFORMATIONTYPE</code> must state a value for the Content Information Type Specification used.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP64"></a><strong>CSIP64</strong>
</td>
      <td>
<strong>Description of the use of the file group</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> <br> The value in the <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> is the name of the whole folder structure to the data, e.g “Documentation”, “Schemas”, “Representations/preingest” or “Representations/submission/data”.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP65"></a><strong>CSIP65</strong>
</td>
      <td>
<strong>File group identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the file group used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP66"></a><strong>CSIP66</strong>
</td>
      <td>
<strong>File</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file</code> <br> The file group (<code class="language-plaintext highlighter-rouge">&lt;fileGrp&gt;</code>) contains the file elements which describe the file objects.</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP67"></a><strong>CSIP67</strong>
</td>
      <td>
<strong>File identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@ID</code> <br> A unique <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for this file across the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP68"></a><strong>CSIP68</strong>
</td>
      <td>
<strong>File mimetype</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@MIMETYPE</code> <br> The IANA mime type for the referenced file. <br> <strong>See also:</strong> <a href="#VocabularyIANAmediaTypes">IANA media types</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP69"></a><strong>CSIP69</strong>
</td>
      <td>
<strong>File size</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@SIZE</code> <br> Size of the referenced file in bytes.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP70"></a><strong>CSIP70</strong>
</td>
      <td>
<strong>File creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@CREATED</code> <br> Creation date of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP71"></a><strong>CSIP71</strong>
</td>
      <td>
<strong>File checksum</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@CHECKSUM</code> <br> The checksum of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP72"></a><strong>CSIP72</strong>
</td>
      <td>
<strong>File checksum type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@CHECKSUMTYPE</code> <br> The type of checksum following the value list present in the METS-standard which has been used for calculating the checksum for the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP73"></a><strong>CSIP73</strong>
</td>
      <td>
<strong>File original identfication</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@OWNERID</code> <br> If an identifier for the file was supplied by the owner it can be recorded in this attribute.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP74"></a><strong>CSIP74</strong>
</td>
      <td>
<strong>File reference to administrative metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@ADMID</code> <br> If administrative metadata has been provided for the file this attribute refers to the file’s administrative metadata by ID.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP75"></a><strong>CSIP75</strong>
</td>
      <td>
<strong>File reference to descriptive metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@DMDID</code> <br> If descriptive metadata has been provided per file this attribute refers to the file’s descriptive metadata by ID.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP76"></a><strong>CSIP76</strong>
</td>
      <td>
<strong>File locator reference</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/FLocat</code> <br> The location of each external file must be defined by the file location <code class="language-plaintext highlighter-rouge">&lt;FLocat&gt;</code> element using the same rules as for referencing metadata files. All references to files should be made using the XLink href attribute and the file protocol using the relative location of the file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP77"></a><strong>CSIP77</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/FLocat[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP78"></a><strong>CSIP78</strong>
</td>
      <td>
<strong>Type of link</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/FLocat[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP79"></a><strong>CSIP79</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/FLocat/@xlink:href</code> <br> The actual location of the resource. We  recommend recording a URL type filepath within this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
  </tbody>
</table>

<p><strong>Example:</strong> METS example of how the structuring of the data is made in the file section</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:fileSec</span> <span class="na">ID=</span><span class="s">"file-sec-example"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"file-grp-doc"</span> <span class="na">USE=</span><span class="s">"Documentation"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file-docx"</span> <span class="na">MIMETYPE=</span><span class="s">"application/vnd.openxmlformats-officedocument.wordprocessingml.document"</span> <span class="na">SIZE=</span><span class="s">"2554366"</span> <span class="na">CREATED=</span><span class="s">"2012-08-15T12:08:15.432+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"91B7A2C0A1614AA8F3DAF11DB4A1C981F14BAA25E6A0336F715B7C513E7A1557"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"documentation/File.docx"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file2-docx"</span> <span class="na">MIMETYPE=</span><span class="s">"application/vnd.openxmlformats-officedocument.wordprocessingml.document"</span> <span class="na">SIZE=</span><span class="s">"2554366"</span> <span class="na">CREATED=</span><span class="s">"2012-08-15T12:08:15.432+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"91B7A2C0A1614AA8F3DAF11DB4A1C981F14BAA25E6A0336F715B7C513E7A1557"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"documentation/File2.docx"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
  <span class="nt">&lt;/mets:fileGrp&gt;</span>
  <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"file-grp-schema"</span> <span class="na">USE=</span><span class="s">"Schemas"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file-ead-schema"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xsd"</span> <span class="na">SIZE=</span><span class="s">"123917"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"0BF9E16ADE296EF277C7B8E5D249D300F1E1EB59F2DCBD89644B676D66F72DCC"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"schemas/ead2002.xsd"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
  <span class="nt">&lt;/mets:fileGrp&gt;</span>
  <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"file-grp-rep-subdata"</span> <span class="na">USE=</span><span class="s">"Representations/submission/data"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"SIARDDK"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file-siard-xml"</span> <span class="na">MIMETYPE=</span><span class="s">"xml"</span> <span class="na">SIZE=</span><span class="s">"1338744"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"7176A627870CFA3854468EC43C5A56F9BD8B30B50A983B8162BF56298A707667"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">ADMID=</span><span class="s">"digiprov-premis-file-2 digiprov-premis-file-1"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/submission/data/SIARD.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
  <span class="nt">&lt;/mets:fileGrp&gt;</span>
<span class="nt">&lt;/mets:fileSec&gt;</span>
</code></pre></div></div>

<p><strong>Example:</strong> METS example of how the structuring of the data including representations are made in the file section</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:fileSec</span> <span class="na">ID=</span><span class="s">"file-sec-example"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"file-grp-doc"</span> <span class="na">USE=</span><span class="s">"Documentation"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file-docx"</span> <span class="na">MIMETYPE=</span><span class="s">"application/vnd.openxmlformats-officedocument.wordprocessingml.document"</span> <span class="na">SIZE=</span><span class="s">"2554366"</span> <span class="na">CREATED=</span><span class="s">"2012-08-15T12:08:15.432+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"91B7A2C0A1614AA8F3DAF11DB4A1C981F14BAA25E6A0336F715B7C513E7A1557"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"documentation/File.docx"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file2-docx"</span> <span class="na">MIMETYPE=</span><span class="s">"application/vnd.openxmlformats-officedocument.wordprocessingml.document"</span> <span class="na">SIZE=</span><span class="s">"2554366"</span> <span class="na">CREATED=</span><span class="s">"2012-08-15T12:08:15.432+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"91B7A2C0A1614AA8F3DAF11DB4A1C981F14BAA25E6A0336F715B7C513E7A1557"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"documentation/File2.docx"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
  <span class="nt">&lt;/mets:fileGrp&gt;</span>
  <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"file-grp-schema"</span> <span class="na">USE=</span><span class="s">"Schemas"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file-ead-schema"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xsd"</span> <span class="na">SIZE=</span><span class="s">"123917"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"0BF9E16ADE296EF277C7B8E5D249D300F1E1EB59F2DCBD89644B676D66F72DCC"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"schemas/ead2002.xsd"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
  <span class="nt">&lt;/mets:fileGrp&gt;</span>
  <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"file-grp-rep-preing"</span> <span class="na">USE=</span><span class="s">"Representations/preingest"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"OTHER"</span> <span class="na">csip:OTHERCONTENTINFORMATIONTYPE=</span><span class="s">"Access database"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file-preing-mets-xml"</span> <span class="na">MIMETYPE=</span><span class="s">"xml"</span> <span class="na">SIZE=</span><span class="s">"1338744"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"7176A627870CFA3854468EC43C5A56F9BD8B30B50A983B8162BF56298A707667"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">ADMID=</span><span class="s">"digiprov-premis-file-2 digiprov-premis-file-1"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/preingest/METS.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
  <span class="nt">&lt;/mets:fileGrp&gt;</span>
  <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"file-grp-rep-sub"</span> <span class="na">USE=</span><span class="s">"Representations/submission"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"SIARDDK"</span> <span class="na">ADMID=</span><span class="s">"digiprov-premis-file-1 digiprov-premis-file-2"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file-sub-mets-xml"</span> <span class="na">MIMETYPE=</span><span class="s">"application/xml"</span> <span class="na">SIZE=</span><span class="s">"1338744"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"7176A627870CFA3854468EC43C5A56F9BD8B30B50A983B8162BF56298A707667"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">ADMID=</span><span class="s">"digiprov-premis-file-2 digiprov-premis-file-1"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/submission/METS.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
  <span class="nt">&lt;/mets:fileGrp&gt;</span>
  <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"file-grp-rep-ing"</span> <span class="na">USE=</span><span class="s">"Representations/ingest"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"SIARD1"</span> <span class="na">ADMID=</span><span class="s">"digiprov-premis-file-3 digiprov-premis-file-4"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"file-ing-mets-xml"</span> <span class="na">MIMETYPE=</span><span class="s">"application/xml"</span> <span class="na">SIZE=</span><span class="s">"1338744"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"7176A627870CFA3854468EC43C5A56F9BD8B30B50A983B8162BF56298A707667"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">ADMID=</span><span class="s">"digiprov-premis-file-2 digiprov-premis-file-1"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/ingest/METS.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:FLocat&gt;</span>
    <span class="nt">&lt;/mets:file&gt;</span>
  <span class="nt">&lt;/mets:fileGrp&gt;</span>
<span class="nt">&lt;/mets:fileSec&gt;</span>
</code></pre></div></div>

<p><a name="useofthemetsstructuralmap%60&lt;structmap&gt;%60"></a></p>

<h3 id="536-use-of-the-mets-structural-map-structmap">5.3.6. Use of the METS structural map (<code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code>)</h3>
<p>The METS structural map element is the only mandatory element in the METS specification. It provides an overview of the components described in the METS document. It can also link the elements in the structure to associated content files and metadata. In the CSIP the <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> describes the higher level structure of all the content in the package and may link to representations.</p>

<p>The CSIP requires the inclusion of one mandatory structural map according to the principles described below.
However, implementers are welcome to define additional structural maps for their internal purposes by repeating the <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> element.
The most crucial requirements for the CSIP mandated structural map are as follows:</p>

<ul>
  <li>The <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> element’s <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute is mandatory and must have the value “CSIP”. The <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute distinguishes the CSIP mandated structural maps from other structural maps. NOTE this means that the “CSIP” <code class="language-plaintext highlighter-rouge">@LABEL</code> value should be treated as a unique id and not applied to other <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> elements;</li>
  <li>The package structure is documented using METS division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> elements which can be arranged in nested tree structures. The CSIP organises it’s constituent <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> elements in a single root structural <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element.
    <ul>
      <li>This top level structural <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element must use the package identifier as the value of its <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute.</li>
    </ul>
  </li>
  <li>The internal structure of the structural map (expressed by <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> elements) follows the CSIP high level physical structure described in Section 4, and groups metadata, representations, schemas, documentation and user-defined folders into discrete <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> elements;
    <ul>
      <li>All <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> elements must have an <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute with the value identical to the folder name, e.g. “metadata”;</li>
    </ul>
  </li>
  <li>When both package and representation METS files are present, the structural map in the Package METS document:
    <ul>
      <li>References the <code class="language-plaintext highlighter-rouge">&lt;fileGrp&gt;</code> which describes every file in every folder, with the exception of the content of the representation folders</li>
      <li>Lists all representations (as separate <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> elements)</li>
      <li>Lists only the appropriate representation METS file using the <code class="language-plaintext highlighter-rouge">&lt;mptr&gt;</code> element as the content of the representation</li>
    </ul>
  </li>
  <li>The structural map in the representations METS file uses the structural map in an identical manner, describing all representation structural map with no exceptions</li>
</ul>

<p>The specific requirements for elements, sub-elements and attributes are listed in the following table. Note that the <code class="language-plaintext highlighter-rouge">&lt;area&gt;</code>, <code class="language-plaintext highlighter-rouge">&lt;seq&gt;</code> and <code class="language-plaintext highlighter-rouge">&lt;par&gt;</code> elements are not discussed below.</p>

<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Name, Location &amp; Description</th>
      <th>Card &amp; Level</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
<a name="CSIP80"></a><strong>CSIP80</strong>
</td>
      <td>
<strong>Structural description of the package</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap</code> <br> The structural map <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> element is the only mandatory element in the METS. <br> The <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> in the CSIP describes the highest logical structure of the IP. <br> Each METS file must include ONE structural map <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> element used exactly as described here. <br> Institutions can add their own additional custom structural maps as separate <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> sections.</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP81"></a><strong>CSIP81</strong>
</td>
      <td>
<strong>Type of structural description</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@TYPE='PHYSICAL']</code> <br> The <code class="language-plaintext highlighter-rouge">mets/structMap/@TYPE</code> attribute must take the value “PHYSICAL” from the vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStructMapType">Structural map typing</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP82"></a><strong>CSIP82</strong>
</td>
      <td>
<strong>Name of the structural description</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']</code> <br> The <code class="language-plaintext highlighter-rouge">mets/structMap/@LABEL</code> attribute value is set to “CSIP” from the vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStructMapLabel">Structural map label</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP83"></a><strong>CSIP83</strong>
</td>
      <td>
<strong>Structural description identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the structural description (structMap) used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP84"></a><strong>CSIP84</strong>
</td>
      <td>
<strong>Main structural division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div</code> <br> The structural map comprises a single division.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP85"></a><strong>CSIP85</strong>
</td>
      <td>
<strong>Main structural division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP86"></a><strong>CSIP86</strong>
</td>
      <td>
<strong>Main structural division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/@LABEL</code> <br> The package’s top-level structural division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element’s <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute value must be identical to the package identifier, i.e. the same value as the <code class="language-plaintext highlighter-rouge">mets/@OBJID</code> attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP88"></a><strong>CSIP88</strong>
</td>
      <td>
<strong>Metadata division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']</code> <br> The metadata referenced in the administrative and/or descriptive metadata section is described in the structural map with one sub division. <br> When the transfer consists of only administrative and/or descriptive metadata this is the only sub division that occurs.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP89"></a><strong>CSIP89</strong>
</td>
      <td>
<strong>Metadata division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP90"></a><strong>CSIP90</strong>
</td>
      <td>
<strong>Metadata division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']</code> <br> The metadata division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element’s <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute value must be “Metadata”. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP91"></a><strong>CSIP91</strong>
</td>
      <td>
<strong>Metadata division administrative metadata referencing</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']/@ADMID</code> <br> When there is administrative metadata and the amdSec is present, all administrative metadata MUST be referenced via the administrative sections different identifiers. <br> All of the <code class="language-plaintext highlighter-rouge">&lt;amdSec&gt;</code> identifiers are listed in a single <code class="language-plaintext highlighter-rouge">@ADMID</code> using spaces as delimiters.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP92"></a><strong>CSIP92</strong>
</td>
      <td>
<strong>Metadata division descriptive metadata referencing</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']/@DMDID</code> <br> When there are descriptive metadata and one or more dmdSec is present, all descriptive metadata MUST be referenced via the descriptive section identifiers. <br> Every <code class="language-plaintext highlighter-rouge">&lt;dmdSec&gt;</code> identifier is listed in a single <code class="language-plaintext highlighter-rouge">@DMDID</code> attribute using spaces as delimiters.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP93"></a><strong>CSIP93</strong>
</td>
      <td>
<strong>Documentation division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']</code> <br> The documentation referenced in the file section file groups is described in the structural map with one sub division.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP94"></a><strong>CSIP94</strong>
</td>
      <td>
<strong>Documentation division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP95"></a><strong>CSIP95</strong>
</td>
      <td>
<strong>Documentation division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']</code> <br> The documentation division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element in the package uses the value “Documentation” from the vocabulary as the value for the <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP96"></a><strong>CSIP96</strong>
</td>
      <td>
<strong>Documentation file referencing</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']/fptr</code> <br> All file groups containing documentation described in the package are referenced via the relevant file group identifiers. There MUST be one file group reference per <code class="language-plaintext highlighter-rouge">&lt;fptr&gt;</code> element.</td>
      <td>
<strong>0..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP116"></a><strong>CSIP116</strong>
</td>
      <td>
<strong>Documentation file group reference pointer</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']/fptr/@FILEID</code> <br> A reference, by ID, to the “Documentation” file group. <br> Related to the requirements CSIP60 which describes the “Documentation” file group and CSIP65 which describes the file group identifier.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP97"></a><strong>CSIP97</strong>
</td>
      <td>
<strong>Schema division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']</code> <br> The schemas referenced in the file section file groups are described in the structural map within a single sub-division.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP98"></a><strong>CSIP98</strong>
</td>
      <td>
<strong>Schema division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP99"></a><strong>CSIP99</strong>
</td>
      <td>
<strong>Schema division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']</code> <br> The schema division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element’s <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute has the value “Schemas” from the vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP100"></a><strong>CSIP100</strong>
</td>
      <td>
<strong>Schema file reference</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']/fptr</code> <br> All file groups containing schemas described in the package are referenced via the relevant file group identifiers. One file group reference per fptr-element</td>
      <td>
<strong>0..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP118"></a><strong>CSIP118</strong>
</td>
      <td>
<strong>Schema file group reference</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']/fptr/@FILEID</code> <br> The pointer to the identifier for the “Schema” file group. <br> Related to the requirements CSIP113 which describes the “Schema” file group and CSIP65 which describes the file group identifier.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP101"></a><strong>CSIP101</strong>
</td>
      <td>
<strong>Content division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']</code> <br> When no representations are present the content referenced in the file section file group with <code class="language-plaintext highlighter-rouge">@USE</code> attribute value “Representations” is described in the structural map as a single sub division.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP102"></a><strong>CSIP102</strong>
</td>
      <td>
<strong>Content division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP103"></a><strong>CSIP103</strong>
</td>
      <td>
<strong>Content division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']</code> <br> The package’s content division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element must have the <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute value “Representations”, taken from the vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP104"></a><strong>CSIP104</strong>
</td>
      <td>
<strong>Content division file references</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']/fptr</code> <br> All file groups containing content described in the package are referenced via the relevant file group identifiers. One file group reference per fptr-element.</td>
      <td>
<strong>0..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP119"></a><strong>CSIP119</strong>
</td>
      <td>
<strong>Content division file group references</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']/fptr/@FILEID</code> <br> The pointer to the identifier for the “Representations” file group. <br> Related to the requirements CSIP114 which describes the “Representations” file group and CSIP65 which describes the file group identifier.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP105"></a><strong>CSIP105</strong>
</td>
      <td>
<strong>Representation division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div</code> <br> When a package consists of multiple representations, each described by a representation level METS.xml document, there is a discrete representation div element for each representation. <br> Each representation div references the representation level METS.xml document, documenting the structure of the package and its constituent representations.</td>
      <td>
<strong>0..n</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP106"></a><strong>CSIP106</strong>
</td>
      <td>
<strong>Representations division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP107"></a><strong>CSIP107</strong>
</td>
      <td>
<strong>Representations division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div/@LABEL</code> <br> The package’s representation division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute value must be the path to the representation level METS document. <br> This requirement gives the same value to be used as the requirement named “File group identifier” (CSIP64) <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP108"></a><strong>CSIP108</strong>
</td>
      <td>
<strong>Representations division file referencing</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div/mptr/@xlink:title</code> <br> The file group containing the files described in the package are referenced via the relevant file group identifier. <br> Related to the requirements CSIP114 which describes the “Representations” file group and CSIP65 which describes the file group identifier.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP109"></a><strong>CSIP109</strong>
</td>
      <td>
<strong>Representation METS pointer</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div/mptr</code> <br> The division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> of the specific representation includes one occurrence of the METS pointer <code class="language-plaintext highlighter-rouge">&lt;mptr&gt;</code> element, pointing to the appropriate representation METS file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP110"></a><strong>CSIP110</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap/div/div/mptr/@xlink:href</code> <br> The actual location of the resource. We  recommend recording a URL type filepath within this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP111"></a><strong>CSIP111</strong>
</td>
      <td>
<strong>Type of link</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap/div/div/mptr[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP112"></a><strong>CSIP112</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap/div/div/mptr[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
  </tbody>
</table>

<p><strong>Example:</strong> METS example of the mandatory structural map</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:structMap</span> <span class="na">ID=</span><span class="s">"struct-map-example-1"</span> <span class="na">TYPE=</span><span class="s">"PHYSICAL"</span> <span class="na">LABEL=</span><span class="s">"CSIP"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-example-div"</span> <span class="na">LABEL=</span><span class="s">"csip-mets-example"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-metadata-div"</span> <span class="na">LABEL=</span><span class="s">"Metadata"</span> <span class="na">ADMID=</span><span class="s">"digiprov-premis-file-1 digiprov-premis-file-2"</span> <span class="na">DMDID=</span><span class="s">"dmd-ead-file"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-doc-div"</span> <span class="na">LABEL=</span><span class="s">"Documentation"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:fptr</span> <span class="na">FILEID=</span><span class="s">"file-ptr-doc"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:fptr&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-schema-div"</span> <span class="na">LABEL=</span><span class="s">"Schemas"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:fptr</span> <span class="na">FILEID=</span><span class="s">"file-grp-schema"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:fptr&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-reps-sub-div"</span> <span class="na">LABEL=</span><span class="s">"Representations"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:fptr</span> <span class="na">FILEID=</span><span class="s">"file-grp-rep-subdata"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:fptr&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
  <span class="nt">&lt;/mets:div&gt;</span>
<span class="nt">&lt;/mets:structMap&gt;</span>
</code></pre></div></div>

<p><strong>Example:</strong> METS example of the mandatory structural map including representations</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:structMap</span> <span class="na">ID=</span><span class="s">"struct-map-example-1"</span> <span class="na">TYPE=</span><span class="s">"PHYSICAL"</span> <span class="na">LABEL=</span><span class="s">"CSIP"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-example-div"</span> <span class="na">LABEL=</span><span class="s">"csip-mets-example"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-metadata-div"</span> <span class="na">LABEL=</span><span class="s">"Metadata"</span> <span class="na">ADMID=</span><span class="s">"digiprov-premis-file-1 digiprov-premis-file-2 digiprov-premis-file-3 digiprov-premis-file-4"</span> <span class="na">DMDID=</span><span class="s">"dmd-ead-file"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-schema-div"</span> <span class="na">LABEL=</span><span class="s">"Schemas"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:fptr</span> <span class="na">FILEID=</span><span class="s">"file-ptr-schema"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:fptr&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-reps-preing-div"</span> <span class="na">LABEL=</span><span class="s">"Representations/preingest"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:mptr</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/preingest/METS.xml"</span> <span class="na">xlink:title=</span><span class="s">"file-grp-rep-preing"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:mptr&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-reps-sub-div"</span> <span class="na">LABEL=</span><span class="s">"Representations/submission"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:mptr</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/submission/METS.xml"</span> <span class="na">xlink:title=</span><span class="s">"file-grp-rep-sub"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:mptr&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"struct-map-reps-ing-div"</span> <span class="na">LABEL=</span><span class="s">"Representations/ingest"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:mptr</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/ingest/METS.xml"</span> <span class="na">xlink:title=</span><span class="s">"file-grp-rep-ing"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:mptr&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
  <span class="nt">&lt;/mets:div&gt;</span>
<span class="nt">&lt;/mets:structMap&gt;</span>
</code></pre></div></div>

<p><a name="useofpremis"></a></p>

<h2 id="54-use-of-premis">5.4. Use of PREMIS</h2>
<p>The CSIP recommends and advocates the use of the PREservation Metadata Implementation Strategies (PREMIS, <a href="http://www.loc.gov/standards/premis/">http://www.loc.gov/standards/premis/</a>) metadata standard for recording preservation and technical metadata about digital objects contained within CSIP Information Packages. The CSIP implements version 3.0 of the PREMIS Data Dictionary. Note that use of PREMIS is not mandatory.</p>

<p>It is strongly recommended that PREMIS metadata is kept in discrete PREMIS XML files inside the IP. The PREMIS metadata can be included in the IP in separate files, and there is no convention regarding the naming and numbering of the PREMIS files. Implementations can choose to either store all preservation metadata in a single PREMIS file or split them into multiple files. In this case, the only requirement is that all PREMIS files must be listed in the appropriate METS file, i.e. package PREMIS files from the package METS file and representation PREMIS files from the representation METS files, and referenced in the METS file(s) using the mdRef attributes and elements.</p>

<p>Therefore, the main recommendation of the CSIP is that preservation metadata are included in the information package in PREMIS format. Although this is not mandatory, all tools that claim to be able to validate CSIP compliant Information Packages must also be able to validate PREMIS metadata once it exists within the package. The two high-level requirements for using PREMIS in Common Specification IPs are that:</p>

<ul>
  <li>
    <p>All preservation metadata is created according to official PREMIS guidelines;</p>
  </li>
  <li>
    <p>All PREMIS metadata is referenced from the amdSec/digiprovMD element of the appropriate METS file.</p>
  </li>
</ul>

<p>Further, to enhance the interoperability scope of the CSIP and to strengthen the management of IPs in an archive, this specification imposes additional requirements with regard to use of PREMIS for describing Information Packages. The principles adopted in the CSIP for deciding the additional PREMIS semantic units required are:</p>

<ul>
  <li>
    <p>PREMIS should be used to record detailed technical metadata;</p>
  </li>
  <li>
    <p>Technical information should be included in PREMIS metadata by using the possibility of extension schemas in PREMIS;</p>
  </li>
  <li>
    <p>Information about agents carrying out preservation actions must be recorded in the PREMIS metadata (e.g. the METS agents describe agents that are relevant for generic IP level events, such as the creation or submission of the package);</p>
  </li>
  <li>
    <p>Event descriptions should be included in PREMIS metadata. Use of the official PREMIS event vocabulary (<a href="http://id.loc.gov/vocabulary/preservation/eventType.html">http://id.loc.gov/vocabulary/preservation/eventType.html</a>) is recommended;</p>
  </li>
  <li>
    <p>Detailed rights information should be included in PREMIS. High-level rights information in METS indicates restrictions. Detailed, object-specific, rights information will be included in the PREMIS metadata;</p>
  </li>
  <li>
    <p>File format information for all files should be included as PUID values in the appropriate PREMIS semantic units.</p>
  </li>
</ul>

<p><a name="vocabularies"></a></p>

<h3 id="541-vocabularies">5.4.1. Vocabularies</h3>

<p>This specification does not present a definitive list of vocabularies for use with PREMIS semantic units but does recommend the use of the Library of Congress vocabularies developed specifically to provide values for various PREMIS semantic units. All relevant vocabularies are presented in the PREMIS Data Dictionary.</p>

<p><a name="identifiers"></a></p>

<h3 id="542-identifiers">5.4.2. Identifiers</h3>

<p>In PREMIS each of the entities (objects, events, agents, rights) are identified by a generic set of identifier containers. These containers follow an identical syntax and structure consisting of an [entity]Identifier container holding two semantic units:</p>

<ul>
  <li>[entity]IdentifierType</li>
  <li>[entity]IdentifierValue</li>
</ul>

<p>The PREMIS data dictionary recognises that the use of identifier types is an implementation-specific issue and does not recommend or require particular vocabularies for identifier types. The Library of Congress has a Standard Identifiers Scheme: <a href="http://id.loc.gov/vocabulary/identifiers.html">http://id.loc.gov/vocabulary/identifiers.html</a> and the CSIP recommends its use in lieu of implementation-specific vocabularies.</p>

<p><a name="implementationconsiderations"></a></p>

<h1 id="6-implementation-considerations">6. Implementation Considerations</h1>
<p>This section touches on some additional issues which are relevant in respect to implementing the CSIP in real-life scenarios.</p>

<p><a name="contentinformationtypespecifications"></a></p>

<h2 id="61-content-information-type-specifications">6.1. Content Information Type Specifications</h2>

<p><a name="whatisacontentinformationtypespecification?"></a></p>

<h3 id="611-what-is-a-content-information-type-specification">6.1.1. What is a Content Information Type Specification?</h3>
<p>A Content Information Type Specification is a mechanism used to extend the scope of the CSIP by defining additional requirements for specific Content Information Types. The OAIS Reference Model defines Content Information as “A set of information that is the original target of preservation, or that includes part or all of that information. It is an Information Object composed of its Content Data Object and its Representation Information”.</p>

<p>Content Information Types can be regarded as categories of Content Information (e.g. relational databases, scientific data or digitised maps). A Content Information Type Specification defines the format and structure, mainly in regard to the Information Object, within an Information Package. This facilitates interoperability when exchanging specific Content Information Types.</p>

<p>The following elements should be at the core of a Content Information Type Specification:</p>

<ul>
  <li>Required file formats for content data;</li>
  <li>Specification of the information package structure (i.e. specific sub-folders under the “data” folder for particular categories of content data);</li>
  <li>Requirements for specific representation metadata that should be available in PREMIS for understanding and rendering the Content Data Object;</li>
  <li>Details of specific (binary) documentation or other components (e.g. software, emulators, etc.) which must be available for rendering and understanding the Content Data Object.</li>
</ul>

<p>Pragmatically it may not be sufficient to deal only with the Information Object. For complex Content Information Types or large IPs, it may be necessary to provide explicit requirements for other metadata relevant to the specific content type. For example, the ERMS Content Information Type Specification prescribes a method for referencing data (i.e. computer files) from descriptive metadata in ERMS format, ensuring package integrity. Stating these requirements in a general specification allows archival institutions receiving SIPs, including ERMS extracts or whole systems to understand and validate potentially complex information packages.</p>

<p>Content Information Type Specifications can be domain-specific, and there may be multiple specifications to cover a particular domain. For example, archival institutions might define a Content Information Type Specification for archiving web sites with descriptive metadata in EAD format, while libraries might define a specification for archiving web sites with MARC metadata.</p>

<p><a name="maintainingcontentinformationtypespecifications"></a></p>

<h3 id="612-maintaining-content-information-type-specifications">6.1.2. Maintaining Content Information Type Specifications</h3>
<p>It is hoped that many Content Information Type Specifications will be developed with the wider community to create new specifications for domains of interest to them. The DILCIS Board aims to work with the community to maintain a list of available specifications following some simple principles:</p>

<ul>
  <li>The DILCIS Board is responsible for establishing reasonable guidelines and quality requirements for new Content Information Type Specifications, and publishing these on the Board website;</li>
  <li>The Board has the responsibility and mandate to manage a registry of available Content Information Type Specifications which meet the guidelines and quality requirements;</li>
  <li>The Board does NOT take ownership of or have responsibility for maintaining and sustaining any Content Information Type Specifications;</li>
  <li>There shall be no limitations to who is allowed to propose additional Content Information Type Specifications; and</li>
  <li>To ensure the quality of available specifications, the Board validates each proposed specification against the guidelines and quality requirements mentioned above. The validation shall be carried out free of charge and within a reasonable time-frame.</li>
</ul>

<p><a name="handlinglargepackages"></a></p>

<h2 id="62-handling-large-packages">6.2. Handling large packages</h2>
<p>By default, a Common Specification IP should be contained in a single folder or archive file. However, the amount of data and metadata within a single IP can easily grow to several GB or even TB and become difficult to manage and inefficient to process (e.g. due to insufficient storage capacity).</p>

<p>The Common Specification can, in principle, be extended in different ways to support the segmentation of large packages into more manageable parts.</p>

<p>The handling of large packages will be specified in a later version of CSIP. Please be aware that this will be a “recommended approach” and, at this point in time, it is not a part of the CSIP instead segmentation of large packages depends on the local implementation. It is also not expected that all tools will support the segmentation of large packages.</p>

<p><a name="handlingdescriptivemetadatawithinthecommonspecification"></a></p>

<h3 id="621-handling-descriptive-metadata-within-the-common-specification">6.2.1. Handling descriptive metadata within the Common Specification</h3>
<p>Descriptive metadata are used to describe the intellectual contents of archival holdings, and they support finding and understanding individual information packages. The CSIP allows essentially for the inclusion of any kind of descriptive metadata in the IP. However, it is required that all descriptive metadata must be placed into the “metadata” folder of the IP, and that it is recommended (should) to also exploit the possibility of creating a specific sub-folder “descriptive” as seen in <a href="#fig11">Figure 11</a> below (cf. EAD.xml).</p>

<p><a name="fig11"></a>
<img src="figs/fig_11_eark_ip_desc_md.svg" alt="CSIP Example" title="EARK IP descriptive metadata."></p>

<p><strong>Figure 11:</strong> E-ARK IP descriptive metadata</p>

<p>Further, all descriptive metadata need to be described in and referenced from METS metadata (i.e. the <code class="language-plaintext highlighter-rouge">METS.xml</code> file) using the element <code class="language-plaintext highlighter-rouge">&lt;dmdSec&gt;</code> (<a href="#fig12">Figure 12</a>) and as such descriptive metadata should not be embedded directly in the METS file.</p>

<p><a name="fig12"></a>
<img src="figs/fig_12_mets_desc_md.svg" alt="METS desc md" title="METS descriptive metadata."></p>

<p><strong>Figure 12:</strong> METS descriptive metadata</p>

<p>Following the requirement of explicitly and physically separating descriptive metadata and data it should be noted that for interoperability purposes appropriate descriptive metadata elements must explicitly refer to the data content they describe (unless the whole data portion is a single intellectual unit described as a discrete set of descriptive metadata). For example, in the case of EAD elements <code class="language-plaintext highlighter-rouge">&lt;dao&gt;</code> and <code class="language-plaintext highlighter-rouge">&lt;daogrp&gt;</code> shall be used to refer to content files from the descriptive metadata. However, regardless of the descriptive metadata standard in question, the references from descriptive metadata must always follow the requirement posed in Section 5.1 above (i.e. create references according to the format defined in RFC 3986, or to express references as a relative path to the data files).</p>

<p>Finally, it is recommended that detailed metadata about intellectual access restrictions and copyright is included in descriptive metadata (i.e. not into the METS or PREMIS portions of the IP).</p>

<p><a name="appendices"></a></p>

<h1 id="7-appendices">7. Appendices</h1>

<p><a name="appendixa:e-arkinformationpackagemetsexamples"></a></p>

<h2 id="71-appendix-a-e-ark-information-package-mets-examples">7.1. Appendix A: E-ARK Information Package METS examples</h2>

<p><strong>Example 1:</strong> Example of a whole METS document describing an information package with no representations</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:mets</span> <span class="na">xmlns:csip=</span><span class="s">"https://DILCIS.eu/XML/METS/CSIPExtensionMETS"</span> <span class="na">xmlns:mets=</span><span class="s">"http://www.loc.gov/METS/"</span> <span class="na">xmlns:xsi=</span><span class="s">"http://www.w3.org/2001/XMLSchema-instance"</span> <span class="na">xmlns:xlink=</span><span class="s">"http://www.w3.org/1999/xlink"</span> <span class="na">OBJID=</span><span class="s">"csip-mets-example"</span> <span class="na">LABEL=</span><span class="s">"Sample CSIP Information Package with no representations"</span> <span class="na">TYPE=</span><span class="s">"Database"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"SIARDDK"</span> <span class="na">PROFILE=</span><span class="s">"https://earkcsip.dilcis.eu/profile/E-ARK-CSIP.xml"</span> <span class="na">xsi:schemaLocation=</span><span class="s">"http://www.loc.gov/METS/ http://www.loc.gov/standards/mets/mets.xsd http://www.w3.org/1999/xlink http://www.loc.gov/standards/mets/xlink.xsd https://DILCIS.eu/XML/METS/CSIPExtensionMETS https://earkcsip.dilcis.eu/schema/DILCISExtensionMETS.xsd"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;mets:metsHdr</span> <span class="na">CREATEDATE=</span><span class="s">"2018-04-24T14:37:49.602+01:00"</span> <span class="na">LASTMODDATE=</span><span class="s">"2018-04-24T14:37:49.602+01:00"</span> <span class="na">RECORDSTATUS=</span><span class="s">"NEW"</span> <span class="na">csip:OAISPACKAGETYPE=</span><span class="s">"SIP"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:agent</span> <span class="na">ROLE=</span><span class="s">"CREATOR"</span> <span class="na">TYPE=</span><span class="s">"OTHER"</span> <span class="na">OTHERTYPE=</span><span class="s">"SOFTWARE"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:name&gt;</span>RODA-in<span class="nt">&lt;/mets:name&gt;</span>
      <span class="nt">&lt;mets:note</span> <span class="na">csip:NOTETYPE=</span><span class="s">"SOFTWARE VERSION"</span><span class="nt">&gt;</span>2.1.0-beta.7<span class="nt">&lt;/mets:note&gt;</span>
    <span class="nt">&lt;/mets:agent&gt;</span>
  <span class="nt">&lt;/mets:metsHdr&gt;</span>
  <span class="nt">&lt;mets:dmdSec</span> <span class="na">ID=</span><span class="s">"appdx1.dmd-ead-file"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.609+01:00"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">MDTYPE=</span><span class="s">"EAD"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"2002"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/descriptive/ead2002.xml"</span> <span class="na">SIZE=</span><span class="s">"903"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.609+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"F24263BF09994749F335E1664DCE0086DB6DCA323FDB6996938BCD28EA9E8153"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;/mets:mdRef&gt;</span>
  <span class="nt">&lt;/mets:dmdSec&gt;</span>
  <span class="nt">&lt;mets:amdSec&gt;</span>
    <span class="nt">&lt;mets:digiprovMD</span> <span class="na">ID=</span><span class="s">"appdx1.digiprov-premis-file-1"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/preservation/premis1.xml"</span> <span class="na">MDTYPE=</span><span class="s">"PREMIS"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"3.0"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xml"</span> <span class="na">SIZE=</span><span class="s">"1211"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"8aa278038dbad54bbf142e7d72b493e2598a94946ea1304dc82a79c6b4bac3d5"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">LABEL=</span><span class="s">"premis1.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:mdRef&gt;</span>
    <span class="nt">&lt;/mets:digiprovMD&gt;</span>
    <span class="nt">&lt;mets:digiprovMD</span> <span class="na">ID=</span><span class="s">"appdx1.digiprov-premis-file-2"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:47:52.783+01:00"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/preservation/premis2.xml"</span> <span class="na">MDTYPE=</span><span class="s">"PREMIS"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"3.0"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xml"</span> <span class="na">SIZE=</span><span class="s">"2854"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"d1dfa585dcc9d87268069dc58d5e47956434ec3db4087a75a3885d287f15126f"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">LABEL=</span><span class="s">"premis2.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:mdRef&gt;</span>
    <span class="nt">&lt;/mets:digiprovMD&gt;</span>
  <span class="nt">&lt;/mets:amdSec&gt;</span>
  <span class="nt">&lt;mets:fileSec</span> <span class="na">ID=</span><span class="s">"appdx1.file-sec-example"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"appdx1.file-grp-doc"</span> <span class="na">USE=</span><span class="s">"Documentation"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx1.file-docx"</span> <span class="na">MIMETYPE=</span><span class="s">"application/vnd.openxmlformats-officedocument.wordprocessingml.document"</span> <span class="na">SIZE=</span><span class="s">"2554366"</span> <span class="na">CREATED=</span><span class="s">"2012-08-15T12:08:15.432+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"91B7A2C0A1614AA8F3DAF11DB4A1C981F14BAA25E6A0336F715B7C513E7A1557"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"documentation/File.docx"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx1.file2-docx"</span> <span class="na">MIMETYPE=</span><span class="s">"application/vnd.openxmlformats-officedocument.wordprocessingml.document"</span> <span class="na">SIZE=</span><span class="s">"2554366"</span> <span class="na">CREATED=</span><span class="s">"2012-08-15T12:08:15.432+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"91B7A2C0A1614AA8F3DAF11DB4A1C981F14BAA25E6A0336F715B7C513E7A1557"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"documentation/File2.docx"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;/mets:fileGrp&gt;</span>
    <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"appdx1.file-grp-schema"</span> <span class="na">USE=</span><span class="s">"Schemas"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx1.file-ead-schema"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xsd"</span> <span class="na">SIZE=</span><span class="s">"123917"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"0BF9E16ADE296EF277C7B8E5D249D300F1E1EB59F2DCBD89644B676D66F72DCC"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"schemas/ead2002.xsd"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;/mets:fileGrp&gt;</span>
    <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"appdx1.file-grp-rep-subdata"</span> <span class="na">USE=</span><span class="s">"Representations/Submission/Data"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"SIARDDK"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx1.file-siard-xml"</span> <span class="na">MIMETYPE=</span><span class="s">"xml"</span> <span class="na">SIZE=</span><span class="s">"1338744"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"7176A627870CFA3854468EC43C5A56F9BD8B30B50A983B8162BF56298A707667"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">ADMID=</span><span class="s">"appdx1.digiprov-premis-file-2 appdx1.digiprov-premis-file-1"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/submission/data/SIARD.xml"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;/mets:fileGrp&gt;</span>
  <span class="nt">&lt;/mets:fileSec&gt;</span>
  <span class="nt">&lt;mets:structMap</span> <span class="na">ID=</span><span class="s">"appdx1.struct-map-example-1"</span> <span class="na">TYPE=</span><span class="s">"PHYSICAL"</span> <span class="na">LABEL=</span><span class="s">"CSIP"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx1.struct-map-example-div"</span> <span class="na">LABEL=</span><span class="s">"csip-mets-example"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx1.struct-map-metadata-div"</span> <span class="na">LABEL=</span><span class="s">"Metadata"</span> <span class="na">ADMID=</span><span class="s">"appdx1.digiprov-premis-file-1 appdx1.digiprov-premis-file-2"</span> <span class="na">DMDID=</span><span class="s">"appdx1.dmd-ead-file"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:div&gt;</span>
      <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx1.struct-map-doc-div"</span> <span class="na">LABEL=</span><span class="s">"Documentation"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:fptr</span> <span class="na">FILEID=</span><span class="s">"appdx1.file-grp-doc"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:fptr&gt;</span>
      <span class="nt">&lt;/mets:div&gt;</span>
      <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx1.struct-map-schema-div"</span> <span class="na">LABEL=</span><span class="s">"Schemas"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:fptr</span> <span class="na">FILEID=</span><span class="s">"appdx1.file-grp-schema"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:fptr&gt;</span>
      <span class="nt">&lt;/mets:div&gt;</span>
      <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx1.struct-map-reps-sub-div"</span> <span class="na">LABEL=</span><span class="s">"Representations"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:fptr</span> <span class="na">FILEID=</span><span class="s">"appdx1.file-grp-rep-subdata"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:fptr&gt;</span>
      <span class="nt">&lt;/mets:div&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
  <span class="nt">&lt;/mets:structMap&gt;</span>
<span class="nt">&lt;/mets:mets&gt;</span>
</code></pre></div></div>

<p><strong>Example 2:</strong> Example of a whole METS document describing an information package with representations</p>

<div class="language-xml highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;mets:mets</span> <span class="na">xmlns:csip=</span><span class="s">"https://DILCIS.eu/XML/METS/CSIPExtensionMETS"</span> <span class="na">xmlns:mets=</span><span class="s">"http://www.loc.gov/METS/"</span> <span class="na">xmlns:xsi=</span><span class="s">"http://www.w3.org/2001/XMLSchema-instance"</span> <span class="na">xmlns:xlink=</span><span class="s">"http://www.w3.org/1999/xlink"</span> <span class="na">OBJID=</span><span class="s">"csip-mets-example"</span> <span class="na">LABEL=</span><span class="s">"Sample CSIP Information Package with representations"</span> <span class="na">TYPE=</span><span class="s">"Database"</span> <span class="na">PROFILE=</span><span class="s">"https://earkcsip.dilcis.eu/profile/E-ARK-CSIP.xml"</span> <span class="na">xsi:schemaLocation=</span><span class="s">"http://www.loc.gov/METS/ http://www.loc.gov/standards/mets/mets.xsd http://www.w3.org/1999/xlink http://www.loc.gov/standards/mets/xlink.xsd https://DILCIS.eu/XML/METS/CSIPExtensionMETS https://earkcsip.dilcis.eu/schema/DILCISExtensionMETS.xsd"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;mets:metsHdr</span> <span class="na">CREATEDATE=</span><span class="s">"2018-04-24T14:37:49.602+01:00"</span> <span class="na">LASTMODDATE=</span><span class="s">"2018-04-24T14:37:49.602+01:00"</span> <span class="na">RECORDSTATUS=</span><span class="s">"NEW"</span> <span class="na">csip:OAISPACKAGETYPE=</span><span class="s">"SIP"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:agent</span> <span class="na">ROLE=</span><span class="s">"CREATOR"</span> <span class="na">TYPE=</span><span class="s">"OTHER"</span> <span class="na">OTHERTYPE=</span><span class="s">"SOFTWARE"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:name&gt;</span>RODA-in<span class="nt">&lt;/mets:name&gt;</span>
      <span class="nt">&lt;mets:note</span> <span class="na">csip:NOTETYPE=</span><span class="s">"SOFTWARE VERSION"</span><span class="nt">&gt;</span>2.1.0-beta.7<span class="nt">&lt;/mets:note&gt;</span>
    <span class="nt">&lt;/mets:agent&gt;</span>
  <span class="nt">&lt;/mets:metsHdr&gt;</span>
  <span class="nt">&lt;mets:dmdSec</span> <span class="na">ID=</span><span class="s">"appdx2.dmd-ead-file"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.609+01:00"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">MDTYPE=</span><span class="s">"EAD"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"2002"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/descriptive/ead2002.xml"</span> <span class="na">SIZE=</span><span class="s">"903"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.609+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"F24263BF09994749F335E1664DCE0086DB6DCA323FDB6996938BCD28EA9E8153"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;/mets:mdRef&gt;</span>
  <span class="nt">&lt;/mets:dmdSec&gt;</span>
  <span class="nt">&lt;mets:amdSec&gt;</span>
    <span class="nt">&lt;mets:digiprovMD</span> <span class="na">ID=</span><span class="s">"appdx2.digiprov-premis-file-1"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/preservation/premis1.xml"</span> <span class="na">MDTYPE=</span><span class="s">"PREMIS"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"3.0"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xml"</span> <span class="na">SIZE=</span><span class="s">"1211"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"8aa278038dbad54bbf142e7d72b493e2598a94946ea1304dc82a79c6b4bac3d5"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">LABEL=</span><span class="s">"premis1.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:mdRef&gt;</span>
    <span class="nt">&lt;/mets:digiprovMD&gt;</span>
    <span class="nt">&lt;mets:digiprovMD</span> <span class="na">ID=</span><span class="s">"appdx2.digiprov-premis-file-2"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:47:52.783+01:00"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/preservation/premis2.xml"</span> <span class="na">MDTYPE=</span><span class="s">"PREMIS"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"3.0"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xml"</span> <span class="na">SIZE=</span><span class="s">"2854"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"d1dfa585dcc9d87268069dc58d5e47956434ec3db4087a75a3885d287f15126f"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">LABEL=</span><span class="s">"premis2.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:mdRef&gt;</span>
    <span class="nt">&lt;/mets:digiprovMD&gt;</span>
    <span class="nt">&lt;mets:digiprovMD</span> <span class="na">ID=</span><span class="s">"appdx2.digiprov-premis-file-3"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/preservation/premis3.xml"</span> <span class="na">MDTYPE=</span><span class="s">"PREMIS"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"3.0"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xml"</span> <span class="na">SIZE=</span><span class="s">"1211"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"8aa278038dbad54bbf142e7d72b493e2598a94946ea1304dc82a79c6b4bac3d5"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">LABEL=</span><span class="s">"premis1.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:mdRef&gt;</span>
    <span class="nt">&lt;/mets:digiprovMD&gt;</span>
    <span class="nt">&lt;mets:digiprovMD</span> <span class="na">ID=</span><span class="s">"appdx2.digiprov-premis-file-4"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:47:52.783+01:00"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:mdRef</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"metadata/preservation/premis4.xml"</span> <span class="na">MDTYPE=</span><span class="s">"PREMIS"</span> <span class="na">MDTYPEVERSION=</span><span class="s">"3.0"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xml"</span> <span class="na">SIZE=</span><span class="s">"2854"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:52.783+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"d1dfa585dcc9d87268069dc58d5e47956434ec3db4087a75a3885d287f15126f"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">LABEL=</span><span class="s">"premis2.xml"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:mdRef&gt;</span>
    <span class="nt">&lt;/mets:digiprovMD&gt;</span>
  <span class="nt">&lt;/mets:amdSec&gt;</span>
  <span class="nt">&lt;mets:fileSec</span> <span class="na">ID=</span><span class="s">"appdx2.file-sec-example"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"appdx2.file-grp-doc"</span> <span class="na">USE=</span><span class="s">"Documentation"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx2.file-docx"</span> <span class="na">MIMETYPE=</span><span class="s">"application/vnd.openxmlformats-officedocument.wordprocessingml.document"</span> <span class="na">SIZE=</span><span class="s">"2554366"</span> <span class="na">CREATED=</span><span class="s">"2012-08-15T12:08:15.432+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"91B7A2C0A1614AA8F3DAF11DB4A1C981F14BAA25E6A0336F715B7C513E7A1557"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"documentation/File.docx"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx2.file2-docx"</span> <span class="na">MIMETYPE=</span><span class="s">"application/vnd.openxmlformats-officedocument.wordprocessingml.document"</span> <span class="na">SIZE=</span><span class="s">"2554366"</span> <span class="na">CREATED=</span><span class="s">"2012-08-15T12:08:15.432+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"91B7A2C0A1614AA8F3DAF11DB4A1C981F14BAA25E6A0336F715B7C513E7A1557"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"documentation/File2.docx"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;/mets:fileGrp&gt;</span>
    <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"appdx2.file-grp-schema"</span> <span class="na">USE=</span><span class="s">"Schemas"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx2.file-ead-schema"</span> <span class="na">MIMETYPE=</span><span class="s">"text/xsd"</span> <span class="na">SIZE=</span><span class="s">"123917"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"0BF9E16ADE296EF277C7B8E5D249D300F1E1EB59F2DCBD89644B676D66F72DCC"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"schemas/ead2002.xsd"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;/mets:fileGrp&gt;</span>
    <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"appdx2.file-grp-rep-preing"</span> <span class="na">USE=</span><span class="s">"Representations/preingest"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"OTHER"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx2.file-preing-mets-xml"</span> <span class="na">MIMETYPE=</span><span class="s">"xml"</span> <span class="na">SIZE=</span><span class="s">"1338744"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"7176A627870CFA3854468EC43C5A56F9BD8B30B50A983B8162BF56298A707667"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">ADMID=</span><span class="s">"appdx2.digiprov-premis-file-2 appdx2.digiprov-premis-file-1"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/preingest/METS.xml"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;/mets:fileGrp&gt;</span>
    <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"appdx2.file-grp-rep-sub"</span> <span class="na">USE=</span><span class="s">"Representations/submission"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"SIARDDK"</span> <span class="na">ADMID=</span><span class="s">"appdx2.digiprov-premis-file-1 appdx2.digiprov-premis-file-2"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx2.file-sub-mets-xml"</span> <span class="na">MIMETYPE=</span><span class="s">"application/xml"</span> <span class="na">SIZE=</span><span class="s">"1338744"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"7176A627870CFA3854468EC43C5A56F9BD8B30B50A983B8162BF56298A707667"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">ADMID=</span><span class="s">"appdx2.digiprov-premis-file-2 appdx2.digiprov-premis-file-1"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/submission/METS.xml"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;/mets:fileGrp&gt;</span>
    <span class="nt">&lt;mets:fileGrp</span> <span class="na">ID=</span><span class="s">"appdx2.file-grp-rep-ing"</span> <span class="na">USE=</span><span class="s">"Representations/ingest"</span> <span class="na">csip:CONTENTINFORMATIONTYPE=</span><span class="s">"SIARD1"</span> <span class="na">ADMID=</span><span class="s">"appdx2.digiprov-premis-file-3 appdx2.digiprov-premis-file-4"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:file</span> <span class="na">ID=</span><span class="s">"appdx2.file-ing-mets-xml"</span> <span class="na">MIMETYPE=</span><span class="s">"application/xml"</span> <span class="na">SIZE=</span><span class="s">"1338744"</span> <span class="na">CREATED=</span><span class="s">"2018-04-24T14:37:49.617+01:00"</span> <span class="na">CHECKSUM=</span><span class="s">"7176A627870CFA3854468EC43C5A56F9BD8B30B50A983B8162BF56298A707667"</span> <span class="na">CHECKSUMTYPE=</span><span class="s">"SHA-256"</span> <span class="na">ADMID=</span><span class="s">"appdx2.digiprov-premis-file-2 appdx2.digiprov-premis-file-1"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:FLocat</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/ingest/METS.xml"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:FLocat&gt;</span>
      <span class="nt">&lt;/mets:file&gt;</span>
    <span class="nt">&lt;/mets:fileGrp&gt;</span>
  <span class="nt">&lt;/mets:fileSec&gt;</span>
  <span class="nt">&lt;mets:structMap</span> <span class="na">ID=</span><span class="s">"appdx2.struct-map-example-1"</span> <span class="na">TYPE=</span><span class="s">"PHYSICAL"</span> <span class="na">LABEL=</span><span class="s">"CSIP"</span><span class="nt">&gt;</span>
    <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx2.struct-map-example-div"</span> <span class="na">LABEL=</span><span class="s">"csip-mets-example"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx2.struct-map-metadata-div"</span> <span class="na">LABEL=</span><span class="s">"Metadata"</span> <span class="na">ADMID=</span><span class="s">"appdx2.digiprov-premis-file-1 appdx2.digiprov-premis-file-2 appdx2.digiprov-premis-file-3 appdx2.digiprov-premis-file-4"</span> <span class="na">DMDID=</span><span class="s">"appdx2.dmd-ead-file"</span><span class="nt">&gt;</span>
      <span class="nt">&lt;/mets:div&gt;</span>
      <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx2.struct-map-schema-div"</span> <span class="na">LABEL=</span><span class="s">"Schemas"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:fptr</span> <span class="na">FILEID=</span><span class="s">"appdx2.file-grp-schema"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:fptr&gt;</span>
      <span class="nt">&lt;/mets:div&gt;</span>
      <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx2.struct-map-reps-preing-div"</span> <span class="na">LABEL=</span><span class="s">"Representations/preingest"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:mptr</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/preingest/METS.xml"</span> <span class="na">xlink:title=</span><span class="s">"file-grp-rep-preing"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:mptr&gt;</span>
      <span class="nt">&lt;/mets:div&gt;</span>
      <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx2.struct-map-reps-sub-div"</span> <span class="na">LABEL=</span><span class="s">"Representations/submission"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:mptr</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/submission/METS.xml"</span> <span class="na">xlink:title=</span><span class="s">"file-grp-rep-sub"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:mptr&gt;</span>
      <span class="nt">&lt;/mets:div&gt;</span>
      <span class="nt">&lt;mets:div</span> <span class="na">ID=</span><span class="s">"appdx2.struct-map-reps-ing-div"</span> <span class="na">LABEL=</span><span class="s">"Representations/ingest"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;mets:mptr</span> <span class="na">LOCTYPE=</span><span class="s">"URL"</span> <span class="na">xlink:type=</span><span class="s">"simple"</span> <span class="na">xlink:href=</span><span class="s">"representations/ingest/METS.xml"</span> <span class="na">xlink:title=</span><span class="s">"file-grp-rep-ing"</span><span class="nt">&gt;</span>
        <span class="nt">&lt;/mets:mptr&gt;</span>
      <span class="nt">&lt;/mets:div&gt;</span>
    <span class="nt">&lt;/mets:div&gt;</span>
  <span class="nt">&lt;/mets:structMap&gt;</span>
<span class="nt">&lt;/mets:mets&gt;</span>
</code></pre></div></div>

<p><a name="appendixb:externalschema"></a></p>

<h2 id="72-appendix-b-external-schema">7.2. Appendix B: External Schema</h2>

<p><a name="e-arkcsipmetsextension"></a></p>

<h3 id="721-e-ark-csip-mets-extension">7.2.1. E-ARK CSIP METS Extension</h3>
<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/DILCISExtensionMETS.xsd">http://earkcsip.dilcis.eu/schema/DILCISExtensionMETS.xsd</a></p>

<p><strong>Context:</strong> XML-schema for the attributes added by CSIP</p>

<p><strong>Note:</strong></p>

<p>An extension schema with the added attributes for use in this profile. <br> 
The schema is identified using the namespace prefix csip. <br></p>

<p><a name="premis"></a></p>

<h3 id="722-premis">7.2.2. PREMIS</h3>
<p><strong>Location:</strong> <a href="http://www.loc.gov/standards/premis/">http://www.loc.gov/standards/premis/</a></p>

<p><strong>Context:</strong> Used for preservation metadata</p>

<p><strong>Note:</strong></p>

<p>A rule set for use with this profile is under development. <br></p>

<p><a name="appendixc:externalvocabularies"></a></p>

<h2 id="73-appendix-c-external-vocabularies">7.3. Appendix C: External Vocabularies</h2>

<p><a name="contentinformationtypespecification"></a></p>

<h3 id="731-content-information-type-specification">7.3.1. Content information type specification</h3>
<p><a name="VocabularyContentInformationTypeSpecification"></a></p>

<p><strong>Maintained By:</strong> DILCIS Board</p>

<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/CSIPVocabularyContentInformationType.xml">http://earkcsip.dilcis.eu/schema/CSIPVocabularyContentInformationType.xml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">@csip:CONTENTINFORMATIONTYPE</code></p>

<p><strong>Description:</strong></p>

<p>Lists the names of specific E-ARK content information type specifications supported or maintained in this METS profile.</p>

<p><a name="contentcategory"></a></p>

<h3 id="732-content-category">7.3.2. Content Category</h3>
<p><a name="VocabularyContentCategory"></a></p>

<p><strong>Maintained By:</strong> DILCIS Board</p>

<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/CSIPVocabularyContentCategory.xml">http://earkcsip.dilcis.eu/schema/CSIPVocabularyContentCategory.xml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">mets/@type</code></p>

<p><strong>Description:</strong></p>

<p>Declares the categorical classification of package content.</p>

<p><a name="oaispackagetype"></a></p>

<h3 id="733-oais-package-type">7.3.3. OAIS Package type</h3>
<p><a name="VocabularyOAISPackageType"></a></p>

<p><strong>Maintained By:</strong> DILCIS Board</p>

<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/CSIPVocabularyOAISPackageType.xml">http://earkcsip.dilcis.eu/schema/CSIPVocabularyOAISPackageType.xml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">@csip:OAISPACKAGETYPE</code></p>

<p><strong>Description:</strong></p>

<p>Describes the OAIS type the package belongs to in the OAIS reference model.</p>

<p><a name="notetype"></a></p>

<h3 id="734-note-type">7.3.4. Note type</h3>
<p><a name="VocabularyNoteType"></a></p>

<p><strong>Maintained By:</strong> DILCIS Board</p>

<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/CSIPVocabularyNoteType.xml">http://earkcsip.dilcis.eu/schema/CSIPVocabularyNoteType.xml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">@csip:NOTETYPE</code></p>

<p><strong>Description:</strong></p>

<p>Provides values for the type of a note for an agent.</p>

<p><a name="otheragenttype"></a></p>

<h3 id="735-other-agent-type">7.3.5. Other agent type</h3>
<p><a name="VocabularyAgentOtherType"></a></p>

<p><strong>Maintained By:</strong> DILCIS Board</p>

<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/CSIPVocabularyAgentOtherType.xml">http://earkcsip.dilcis.eu/schema/CSIPVocabularyAgentOtherType.xml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">metsHdr/agent/@OTHERTYPE</code></p>

<p><strong>Description:</strong></p>

<p>Describes the other agent types supported by the profile.</p>

<p><a name="identifiertype"></a></p>

<h3 id="736-identifier-type">7.3.6. Identifier type</h3>
<p><a name="VocabularyIdentifierType"></a></p>

<p><strong>Maintained By:</strong> Library of Congress</p>

<p><strong>Location:</strong> <a href="http://id.loc.gov/vocabulary/identifiers.html">http://id.loc.gov/vocabulary/identifiers.html</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">metsHdr/altRecordID/@TYPE</code></p>

<p><strong>Description:</strong></p>

<p>Describes the type of the identifier.</p>

<p><a name="dmdsecstatus"></a></p>

<h3 id="737-dmdsec-status">7.3.7. dmdSec status</h3>
<p><a name="VocabularyStatus"></a></p>

<p><strong>Maintained By:</strong> DILCIS Board</p>

<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/CSIPVocabularyStatus.xml">http://earkcsip.dilcis.eu/schema/CSIPVocabularyStatus.xml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">dmdSec/@STATUS</code></p>

<p><strong>Description:</strong></p>

<p>Describes the status of the descriptive metadata section (dmdSec) which is supported by the profile.</p>

<p><a name="ianamediatypes"></a></p>

<h3 id="738-iana-media-types">7.3.8. IANA media types</h3>
<p><a name="VocabularyIANAmediaTypes"></a></p>

<p><strong>Maintained By:</strong> IANAs</p>

<p><strong>Location:</strong> <a href="https://www.iana.org/assignments/media-types/media-types.xhtml">https://www.iana.org/assignments/media-types/media-types.xhtml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">@MIMETYPE</code></p>

<p><strong>Description:</strong></p>

<p>Valid values for the mime types of referenced files.</p>

<p><a name="filegroupnames"></a></p>

<h3 id="739-file-group-names">7.3.9. File group names</h3>
<p><a name="VocabularyFileGrpAndStructMapDivisionLabel"></a></p>

<p><strong>Maintained By:</strong> DILCIS Board</p>

<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/CSIPVocabularyFileGrpAndStructMapDivisionLabel.xml">http://earkcsip.dilcis.eu/schema/CSIPVocabularyFileGrpAndStructMapDivisionLabel.xml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">fileGrp/@USE</code></p>

<p><strong>Description:</strong></p>

<p>Describes the uses of the file group <code class="language-plaintext highlighter-rouge">&lt;fileGrp&gt;</code> that are supported by the profile.<br>
Own names should be placed in an own extending vocabulary.</p>

<p><a name="structuralmaptyping"></a></p>

<h3 id="7310-structural-map-typing">7.3.10. Structural map typing</h3>
<p><a name="VocabularyStructMapType"></a></p>

<p><strong>Maintained By:</strong> DILCIS Board</p>

<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/CSIPVocabularyStructMapType.xml">http://earkcsip.dilcis.eu/schema/CSIPVocabularyStructMapType.xml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">structMap/@TYPE</code></p>

<p><strong>Description:</strong></p>

<p>Describes the type of the structural map <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> that is supported by the profile.<br>
Own types should be placed in an own extending vocabulary.</p>

<p><a name="structuralmaplabel"></a></p>

<h3 id="7311-structural-map-label">7.3.11. Structural map label</h3>
<p><a name="VocabularyStructMapLabel"></a></p>

<p><strong>Maintained By:</strong> DILCIS Board</p>

<p><strong>Location:</strong> <a href="http://earkcsip.dilcis.eu/schema/CSIPVocabularyStructMapLabel.xml">http://earkcsip.dilcis.eu/schema/CSIPVocabularyStructMapLabel.xml</a></p>

<p><strong>Context:</strong> Values for <code class="language-plaintext highlighter-rouge">structMap/@LABEL</code></p>

<p><strong>Description:</strong></p>

<p>Describes the label of the structural map that is supported by the profile.<br>
Own labels should be placed in an own extending vocabulary.</p>

<p><a name="appendixd:afulllistofe-arkcsiprequirements"></a></p>

<h2 id="74-appendix-d-a-full-list-of-e-ark-csip-requirements">7.4. Appendix D: A Full List of E-ARK CSIP Requirements</h2>

<p><a name="structuralrequirements"></a></p>

<h3 id="741-structural-requirements">7.4.1. Structural Requirements</h3>

<p>The implementation requirements of the CSIP Information Package structure are:</p>

<p><a name="CSIPSTR1"></a>
<strong>CSIPSTR1</strong>: Any Information Package <strong>MUST</strong> be included within a single physical root folder (known as the “Information Package root folder”). For packages presented in an archive format, <a href="#CSIPSTR3">see CSIPSTR3</a>, the archive <strong>MUST</strong> unpack to a single root folder.</p>

<p><a name="CSIPSTR2"></a>
<strong>CSIPSTR2</strong>: The Information Package root folder <strong>SHOULD</strong> be named with the ID or name of the Information Package, that is the value of the package METS.xml’s root <code class="language-plaintext highlighter-rouge">&lt;mets&gt;</code> element’s <code class="language-plaintext highlighter-rouge">@OBJID</code> attribute.</p>

<p><a name="CSIPSTR3"></a>
<strong>CSIPSTR3</strong>: The Information Package root folder <strong>MAY</strong> be compressed (for example by using TAR or ZIP). Which specific compression format to use needs to be stated in the Submission Agreement.</p>

<p><a name="CSIPSTR4"></a>
<strong>CSIPSTR4</strong>: The Information Package root folder <strong>MUST</strong> include a file named <code class="language-plaintext highlighter-rouge">METS.xml</code>. This file <strong>MUST</strong> contain metadata that identifies the package, provides a high-level package description, and describes its structure, including pointers to constituent representations.</p>

<p><a name="CSIPSTR5"></a>
<strong>CSIPSTR5</strong>: The Information Package root folder <strong>SHOULD</strong> include a folder named <code class="language-plaintext highlighter-rouge">metadata</code>, which SHOULD include metadata relevant to the whole package.</p>

<p><a name="CSIPSTR6"></a>
<strong>CSIPSTR6</strong>: If preservation metadata are available, they <strong>SHOULD</strong> be included in sub-folder <code class="language-plaintext highlighter-rouge">preservation</code>.</p>

<p><a name="CSIPSTR7"></a>
<strong>CSIPSTR7</strong>: If descriptive metadata are available, they <strong>SHOULD</strong> be included in sub-folder <code class="language-plaintext highlighter-rouge">descriptive</code>.</p>

<p><a name="CSIPSTR8"></a>
<strong>CSIPSTR8</strong>: If any other metadata are available, they <strong>MAY</strong> be included in separate sub-folders, for example an additional folder named <code class="language-plaintext highlighter-rouge">other</code>.</p>

<p><a name="CSIPSTR9"></a>
<strong>CSIPSTR9</strong>: The Information Package folder <strong>SHOULD</strong> include a folder named <code class="language-plaintext highlighter-rouge">representations</code>.</p>

<p><a name="CSIPSTR10"></a>
<strong>CSIPSTR10</strong>: The <code class="language-plaintext highlighter-rouge">representations</code> folder <strong>SHOULD</strong> include a sub-folder for each individual representation (i.e. the “representation folder”). Each representation folder should have a string name that is unique within the package scope. For example the name of the representation and/or its creation date might be good candidates as a representation sub-folder name.</p>

<p><a name="CSIPSTR11"></a>
<strong>CSIPSTR11</strong>: The representation folder <strong>SHOULD</strong> include a sub-folder named <code class="language-plaintext highlighter-rouge">data</code> which <strong>MAY</strong> include all data constituting the representation.</p>

<p><a name="CSIPSTR12"></a>
<strong>CSIPSTR12</strong>: The representation folder <strong>SHOULD</strong> include a metadata file named <code class="language-plaintext highlighter-rouge">METS.xml</code> which includes information about the identity and structure of the representation and its components. The recommended best practice is to always have a <code class="language-plaintext highlighter-rouge">METS.xml</code> in the representation folder.</p>

<p><a name="CSIPSTR13"></a>
<strong>CSIPSTR13</strong>: The representation folder <strong>SHOULD</strong> include a sub-folder named <code class="language-plaintext highlighter-rouge">metadata</code> which <strong>MAY</strong> include all metadata about the specific representation.</p>

<p><a name="CSIPSTR14"></a>
<strong>CSIPSTR14</strong>: The Information Package <strong>MAY</strong> be extended with additional sub-folders.</p>

<p><a name="CSIPSTR15"></a>
<strong>CSIPSTR15</strong>: We recommend including all XML schema documents for any structured metadata within package. These schema documents <strong>SHOULD</strong> be placed in a sub-folder called <code class="language-plaintext highlighter-rouge">schemas</code> within the Information Package root folder and/or the representation folder.</p>

<p><a name="CSIPSTR16"></a>
<strong>CSIPSTR16</strong>: We recommend including any supplementary documentation for the package or a specific representation within the package. Supplementary documentation <strong>SHOULD</strong> be placed in a sub-folder called <code class="language-plaintext highlighter-rouge">documentation</code> within the Information Package root folder and/or the representation folder.</p>

<p><a name="metadatarequirements"></a></p>

<h3 id="742-metadata-requirements">7.4.2. Metadata Requirements</h3>

<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Name, Location &amp; Description</th>
      <th>Card &amp; Level</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
<a name="CSIP1"></a><strong>CSIP1</strong>
</td>
      <td>
<strong>Package Identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/@OBJID</code> <br> The <code class="language-plaintext highlighter-rouge">mets/@OBJID</code> attribute is mandatory, its value is a string identifier for the METS document. For the package METS document, this should be the name/ID of the package, i.e. the name of the package root folder. <br> For a representation level METS document this value records the name/ID of the representation, i.e. the name of the top-level representation folder.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP2"></a><strong>CSIP2</strong>
</td>
      <td>
<strong>Content Category</strong> <br> <code class="language-plaintext highlighter-rouge">mets/@TYPE</code> <br> The <code class="language-plaintext highlighter-rouge">mets/@TYPE</code> attribute MUST be used to declare the category of the content held in the package, e.g. book, journal, stereograph, video, etc.. Legal values are defined in a fixed vocabulary. When the content category used falls outside of the defined vocabulary the <code class="language-plaintext highlighter-rouge">mets/@TYPE</code> value must be set to “OTHER” and the specific value declared in <code class="language-plaintext highlighter-rouge">mets/@csip:OTHERTYPE</code>. The vocabulary will develop under the curation of the DILCIS Board as additional content information type specifications are produced. <br> <strong>See also:</strong> <a href="#VocabularyContentCategory">Content Category</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP3"></a><strong>CSIP3</strong>
</td>
      <td>
<strong>Other Content Category</strong> <br> <code class="language-plaintext highlighter-rouge">mets[@TYPE='OTHER']/@csip:OTHERTYPE</code> <br> When the <code class="language-plaintext highlighter-rouge">mets/@TYPE</code> attribute has the value “OTHER” the <code class="language-plaintext highlighter-rouge">mets/@csip:OTHERTYPE</code> attribute MUST be used to declare the content category of the package/representation. <br> <strong>See also:</strong> <a href="#VocabularyContentCategory">Content Category</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP4"></a><strong>CSIP4</strong>
</td>
      <td>
<strong>Content Information Type Specification</strong> <br> <code class="language-plaintext highlighter-rouge">mets/@csip:CONTENTINFORMATIONTYPE</code> <br> Used to declare the Content Information Type Specification used when creating the package. Legal values are defined in a fixed vocabulary. The attribute is mandatory for representation level METS documents. The vocabulary will evolve under the care of the DILCIS Board as additional Content Information Type Specifications are developed. <br> <strong>See also:</strong> <a href="#VocabularyContentInformationTypeSpecification">Content information type specification</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP5"></a><strong>CSIP5</strong>
</td>
      <td>
<strong>Other Content Information Type Specification</strong> <br> <code class="language-plaintext highlighter-rouge">mets[@csip:CONTENTINFORMATIONTYPE='OTHER']/@csip:OTHERCONTENTINFORMATIONTYPE</code> <br> When the <code class="language-plaintext highlighter-rouge">mets/@csip:CONTENTINFORMATIONTYPE</code> has the value “OTHER” the <code class="language-plaintext highlighter-rouge">mets/@csip:OTHERCONTENTINFORMATIONTYPE</code> must state the content information type.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP6"></a><strong>CSIP6</strong>
</td>
      <td>
<strong>METS Profile</strong> <br> <code class="language-plaintext highlighter-rouge">mets/@PROFILE</code> <br> The URL of the METS profile that the information package conforms with.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP117"></a><strong>CSIP117</strong>
</td>
      <td>
<strong>Package header</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr</code> <br> General element for describing the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP7"></a><strong>CSIP7</strong>
</td>
      <td>
<strong>Package creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@CREATEDATE</code> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@CREATEDATE</code> records the date the package was created.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP8"></a><strong>CSIP8</strong>
</td>
      <td>
<strong>Package last modification date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@LASTMODDATE</code> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@LASTMODDATE</code> is mandatory when the package has been modified.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP9"></a><strong>CSIP9</strong>
</td>
      <td>
<strong>OAIS Package type information</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@csip:OAISPACKAGETYPE</code> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/@csip:OAISPACKAGETYPE</code> is an additional CSIP attribute that declares the type of the IP. <br> <strong>See also:</strong> <a href="#VocabularyOAISPackageType">OAIS Package type</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP10"></a><strong>CSIP10</strong>
</td>
      <td>
<strong>Agent</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent</code> <br> A mandatory agent element records the software used to create the package. Other uses of agents may be described in any local implementations that extend the profile.</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP11"></a><strong>CSIP11</strong>
</td>
      <td>
<strong>Agent role</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent[@ROLE='CREATOR']</code> <br> The mandatory agent element MUST have a <code class="language-plaintext highlighter-rouge">@ROLE</code> attribute with the value “CREATOR”.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP12"></a><strong>CSIP12</strong>
</td>
      <td>
<strong>Agent type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent[@TYPE='OTHER']</code> <br> The mandatory agent element MUST have a <code class="language-plaintext highlighter-rouge">@TYPE</code> attribute with the value “OTHER”.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP13"></a><strong>CSIP13</strong>
</td>
      <td>
<strong>Agent other type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent[@OTHERTYPE='SOFTWARE']</code> <br> The mandatory agent element MUST have a <code class="language-plaintext highlighter-rouge">@OTHERTYPE</code> attribute with the value “SOFTWARE”. <br> <strong>See also:</strong> <a href="#VocabularyAgentOtherType">Other agent type</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP14"></a><strong>CSIP14</strong>
</td>
      <td>
<strong>Agent name</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent/name</code> <br> The mandatory agent’s name element records the name of the software tool used to create the IP.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP15"></a><strong>CSIP15</strong>
</td>
      <td>
<strong>Agent additional information</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent/note</code> <br> The mandatory agent’s note element records the version of the tool used to create the IP.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP16"></a><strong>CSIP16</strong>
</td>
      <td>
<strong>Classification of the agent additional information</strong> <br> <code class="language-plaintext highlighter-rouge">mets/metsHdr/agent/note[@csip:NOTETYPE='SOFTWARE VERSION']</code> <br> The mandatory agent element’s note child has a <code class="language-plaintext highlighter-rouge">@csip:NOTETYPE</code> attribute with a fixed value of “SOFTWARE VERSION”. <br> <strong>See also:</strong> <a href="#VocabularyNoteType">Note type</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP17"></a><strong>CSIP17</strong>
</td>
      <td>
<strong>Descriptive metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec</code> <br> Must be used if descriptive metadata for the package content is available. Each descriptive metadata section (<code class="language-plaintext highlighter-rouge">&lt;dmdSec&gt;</code>) contains a single description and must be repeated for multiple descriptions, when available. <br> It is possible to transfer metadata in a package using just the descriptive metadata section and/or administrative metadata section.</td>
      <td>
<strong>0..n</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP18"></a><strong>CSIP18</strong>
</td>
      <td>
<strong>Descriptive metadata identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the descriptive metadata section (<code class="language-plaintext highlighter-rouge">&lt;dmdSec&gt;</code>) used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP19"></a><strong>CSIP19</strong>
</td>
      <td>
<strong>Descriptive metadata creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/@CREATED</code> <br> Creation date of the descriptive metadata in this section.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP20"></a><strong>CSIP20</strong>
</td>
      <td>
<strong>Status of the descriptive metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/@STATUS</code> <br> Indicates the status of the package using a fixed vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStatus">dmdSec status</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP21"></a><strong>CSIP21</strong>
</td>
      <td>
<strong>Reference to the document with the descriptive metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef</code> <br> Reference to the descriptive metadata file located in the “metadata” section of the IP.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP22"></a><strong>CSIP22</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP23"></a><strong>CSIP23</strong>
</td>
      <td>
<strong>Type of link</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP24"></a><strong>CSIP24</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@xlink:href</code> <br> The actual location of the resource. This specification recommends recording a URL type filepath in this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP25"></a><strong>CSIP25</strong>
</td>
      <td>
<strong>Type of metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@MDTYPE</code> <br> Specifies the type of metadata in the referenced file. Values are taken from the list provided by the METS.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP26"></a><strong>CSIP26</strong>
</td>
      <td>
<strong>File mime type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@MIMETYPE</code> <br> The IANA mime type of the referenced file. <br> <strong>See also:</strong> <a href="#VocabularyIANAmediaTypes">IANA media types</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP27"></a><strong>CSIP27</strong>
</td>
      <td>
<strong>File size</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@SIZE</code> <br> Size of the referenced file in bytes.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP28"></a><strong>CSIP28</strong>
</td>
      <td>
<strong>File creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@CREATED</code> <br> The creation date of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP29"></a><strong>CSIP29</strong>
</td>
      <td>
<strong>File checksum</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@CHECKSUM</code> <br> The checksum of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP30"></a><strong>CSIP30</strong>
</td>
      <td>
<strong>File checksum type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/dmdSec/mdRef/@CHECKSUMTYPE</code> <br> The type of checksum following the value list present in the METS-standard which has been used for calculating the checksum for the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP31"></a><strong>CSIP31</strong>
</td>
      <td>
<strong>Administrative metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec</code> <br> If administrative / preservation metadata is available, it must be described using the administrative metadata section (<code class="language-plaintext highlighter-rouge">&lt;amdSec&gt;</code>) element. <br> All administrative metadata is present in a single <code class="language-plaintext highlighter-rouge">&lt;amdSec&gt;</code> element. <br> It is possible to transfer metadata in a package using just the descriptive metadata section and/or administrative metadata section.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP32"></a><strong>CSIP32</strong>
</td>
      <td>
<strong>Digital provenance metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD</code> <br> For recording information about preservation the standard PREMIS is used. It is mandatory to include one <code class="language-plaintext highlighter-rouge">&lt;digiprovMD&gt;</code> element for each piece of PREMIS metadata. <br> The use if PREMIS in METS is following the recommendations in  <a href="http://www.loc.gov/standards/premis/guidelines2017-premismets.pdf"> the 2017 version of PREMIS in METS Guidelines.</a>
</td>
      <td>
<strong>0..n</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP33"></a><strong>CSIP33</strong>
</td>
      <td>
<strong>Digital provenance metadata identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the digital provenance metadata section <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD</code> used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP34"></a><strong>CSIP34</strong>
</td>
      <td>
<strong>Status of the digital provenance metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/@STATUS</code> <br> Indicates the status of the package using a fixed vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStatus">dmdSec status</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP35"></a><strong>CSIP35</strong>
</td>
      <td>
<strong>Reference to the document with the digital provenance metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef</code> <br> Reference to the digital provenance metadata file stored in the “metadata” section of the IP.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP36"></a><strong>CSIP36</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP37"></a><strong>CSIP37</strong>
</td>
      <td>
<strong>Type of link</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP38"></a><strong>CSIP38</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@xlink:href</code> <br> The actual location of the resource. This specification recommends recording a URL type filepath within this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP39"></a><strong>CSIP39</strong>
</td>
      <td>
<strong>Type of metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@MDTYPE</code> <br> Specifies the type of metadata in the referenced file. Values are taken from the list provided by the METS.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP40"></a><strong>CSIP40</strong>
</td>
      <td>
<strong>File mime type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@MIMETYPE</code> <br> The IANA mime type for the referenced file. <br> <strong>See also:</strong> <a href="#VocabularyIANAmediaTypes">IANA media types</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP41"></a><strong>CSIP41</strong>
</td>
      <td>
<strong>File size</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@SIZE</code> <br> Size of the referenced file in bytes.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP42"></a><strong>CSIP42</strong>
</td>
      <td>
<strong>File creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@CREATED</code> <br> Creation date of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP43"></a><strong>CSIP43</strong>
</td>
      <td>
<strong>File checksum</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@CHECKSUM</code> <br> The checksum of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP44"></a><strong>CSIP44</strong>
</td>
      <td>
<strong>File checksum type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/digiprovMD/mdRef/@CHECKSUMTYPE</code> <br> The type of checksum following the value list present in the METS-standard which has been used for calculating the checksum for the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP45"></a><strong>CSIP45</strong>
</td>
      <td>
<strong>Rights metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD</code> <br> A simple rights statement may be used to describe general permissions for the package. Individual representations should state their specific rights in their representation METS file. <br> Available standards include  <a href="http://rightsstatements.org">RightsStatements.org</a> ,  <a href="https://pro.europeana.eu/page/available-rights-statements">Europeana rights statements info</a> ,  <a href="https://github.com/mets/METS-Rights-Schema">METS Rights Schema</a>  created and maintained by the METS Board, the rights part of  <a href="http://www.loc.gov/standards/premis/">PREMIS</a>  as well as own local rights statements in use.</td>
      <td>
<strong>0..n</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP46"></a><strong>CSIP46</strong>
</td>
      <td>
<strong>Rights metadata identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the rights metadata section (<code class="language-plaintext highlighter-rouge">&lt;rightsMD&gt;</code>) used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP47"></a><strong>CSIP47</strong>
</td>
      <td>
<strong>Status of the rights metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/@STATUS</code> <br> Indicates the status of the package using a fixed vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStatus">dmdSec status</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP48"></a><strong>CSIP48</strong>
</td>
      <td>
<strong>Reference to the document with the rights metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef</code> <br> Reference to the rights metadata file stored in the “metadata” section of the IP.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP49"></a><strong>CSIP49</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP50"></a><strong>CSIP50</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP51"></a><strong>CSIP51</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@xlink:href</code> <br> The actual location of the resource. We  recommend recording a URL type filepath within this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP52"></a><strong>CSIP52</strong>
</td>
      <td>
<strong>Type of metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@MDTYPE</code> <br> Specifies the type of metadata in the referenced file. Value is taken from the list provided by the METS.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP53"></a><strong>CSIP53</strong>
</td>
      <td>
<strong>File mime type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@MIMETYPE</code> <br> The IANA mime type for the referenced file. <br> <strong>See also:</strong> <a href="#VocabularyIANAmediaTypes">IANA media types</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP54"></a><strong>CSIP54</strong>
</td>
      <td>
<strong>File size</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@SIZE</code> <br> Size of the referenced file in bytes.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP55"></a><strong>CSIP55</strong>
</td>
      <td>
<strong>File creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@CREATED</code> <br> Creation date of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP56"></a><strong>CSIP56</strong>
</td>
      <td>
<strong>File checksum</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@CHECKSUM</code> <br> The checksum of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP57"></a><strong>CSIP57</strong>
</td>
      <td>
<strong>File checksum type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/amdSec/rightsMD/mdRef/@CHECKSUMTYPE</code> <br> The type of checksum following the value list present in the METS-standard which has been used for calculating the checksum for the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP58"></a><strong>CSIP58</strong>
</td>
      <td>
<strong>File section</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec</code> <br> The transferred content is placed in the file section in different file group elements, described in other requirements. <br> Only a single file section (<code class="language-plaintext highlighter-rouge">&lt;fileSec&gt;</code>) element should be present. <br> It is possible to transfer just descriptive metadata and/or administrative metadata without files placed in this section.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP59"></a><strong>CSIP59</strong>
</td>
      <td>
<strong>File section identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the file section used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP60"></a><strong>CSIP60</strong>
</td>
      <td>
<strong>Documentation file group</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@USE='Documentation']</code> <br> All documentation pertaining to the transferred content is placed in one or more file group elements with <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> attribute value “Documentation”. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP113"></a><strong>CSIP113</strong>
</td>
      <td>
<strong>Schema file group</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@USE='Schemas']</code> <br> All XML schemas used in the information package should be referenced from one or more file groups with <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> attribute value “Schemas”. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP114"></a><strong>CSIP114</strong>
</td>
      <td>
<strong>Representations file group</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@USE='Representations']</code> <br> A pointer to the METS document describing the representation or pointers to the content being transferred must be present in one or more file groups with <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> attribute value “Representations”. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP61"></a><strong>CSIP61</strong>
</td>
      <td>
<strong>Reference to administrative metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@ADMID</code> <br> If administrative metadata has been provided at file group  <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp</code> level this attribute refers to its administrative metadata section by ID.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP62"></a><strong>CSIP62</strong>
</td>
      <td>
<strong>Content Information Type Specification</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@USE='Representations']/@csip:CONTENTINFORMATIONTYPE</code> <br> An added attribute which states the name of the content information type specification used to create the package. <br> The vocabulary will evolve under the curation of the DILCIS Board as additional content information type specifications are developed. <br> This attribute is mandatory when the <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> attribute value is “Representations”. <br> When the “Package type” value is “Mixed” and/or the file group describes a “Representation”, then this element states the content information type specification used for the file group. <br> <strong>See also:</strong> <a href="#VocabularyContentInformationTypeSpecification">Content information type specification</a>
</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP63"></a><strong>CSIP63</strong>
</td>
      <td>
<strong>Other Content Information Type Specification</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp[@csip:CONTENTINFORMATIONTYPE='OTHER']/@csip:OTHERCONTENTINFORMATIONTYPE</code> <br> When the <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@csip:CONTENTINFORMATIONTYPE</code> attribute has the value “OTHER” the <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@csip:OTHERCONTENTINFORMATIONTYPE</code> must state a value for the Content Information Type Specification used.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP64"></a><strong>CSIP64</strong>
</td>
      <td>
<strong>Description of the use of the file group</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> <br> The value in the <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@USE</code> is the name of the whole folder structure to the data, e.g “Documentation”, “Schemas”, “Representations/preingest” or “Representations/submission/data”.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP65"></a><strong>CSIP65</strong>
</td>
      <td>
<strong>File group identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the file group used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP66"></a><strong>CSIP66</strong>
</td>
      <td>
<strong>File</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file</code> <br> The file group (<code class="language-plaintext highlighter-rouge">&lt;fileGrp&gt;</code>) contains the file elements which describe the file objects.</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP67"></a><strong>CSIP67</strong>
</td>
      <td>
<strong>File identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@ID</code> <br> A unique <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for this file across the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP68"></a><strong>CSIP68</strong>
</td>
      <td>
<strong>File mimetype</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@MIMETYPE</code> <br> The IANA mime type for the referenced file. <br> <strong>See also:</strong> <a href="#VocabularyIANAmediaTypes">IANA media types</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP69"></a><strong>CSIP69</strong>
</td>
      <td>
<strong>File size</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@SIZE</code> <br> Size of the referenced file in bytes.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP70"></a><strong>CSIP70</strong>
</td>
      <td>
<strong>File creation date</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@CREATED</code> <br> Creation date of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP71"></a><strong>CSIP71</strong>
</td>
      <td>
<strong>File checksum</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@CHECKSUM</code> <br> The checksum of the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP72"></a><strong>CSIP72</strong>
</td>
      <td>
<strong>File checksum type</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@CHECKSUMTYPE</code> <br> The type of checksum following the value list present in the METS-standard which has been used for calculating the checksum for the referenced file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP73"></a><strong>CSIP73</strong>
</td>
      <td>
<strong>File original identfication</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@OWNERID</code> <br> If an identifier for the file was supplied by the owner it can be recorded in this attribute.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP74"></a><strong>CSIP74</strong>
</td>
      <td>
<strong>File reference to administrative metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@ADMID</code> <br> If administrative metadata has been provided for the file this attribute refers to the file’s administrative metadata by ID.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP75"></a><strong>CSIP75</strong>
</td>
      <td>
<strong>File reference to descriptive metadata</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/@DMDID</code> <br> If descriptive metadata has been provided per file this attribute refers to the file’s descriptive metadata by ID.</td>
      <td>
<strong>0..1</strong> <br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="CSIP76"></a><strong>CSIP76</strong>
</td>
      <td>
<strong>File locator reference</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/FLocat</code> <br> The location of each external file must be defined by the file location <code class="language-plaintext highlighter-rouge">&lt;FLocat&gt;</code> element using the same rules as for referencing metadata files. All references to files should be made using the XLink href attribute and the file protocol using the relative location of the file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP77"></a><strong>CSIP77</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/FLocat[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP78"></a><strong>CSIP78</strong>
</td>
      <td>
<strong>Type of link</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/FLocat[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP79"></a><strong>CSIP79</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/fileSec/fileGrp/file/FLocat/@xlink:href</code> <br> The actual location of the resource. We  recommend recording a URL type filepath within this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP80"></a><strong>CSIP80</strong>
</td>
      <td>
<strong>Structural description of the package</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap</code> <br> The structural map <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> element is the only mandatory element in the METS. <br> The <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> in the CSIP describes the highest logical structure of the IP. <br> Each METS file must include ONE structural map <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> element used exactly as described here. <br> Institutions can add their own additional custom structural maps as separate <code class="language-plaintext highlighter-rouge">&lt;structMap&gt;</code> sections.</td>
      <td>
<strong>1..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP81"></a><strong>CSIP81</strong>
</td>
      <td>
<strong>Type of structural description</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@TYPE='PHYSICAL']</code> <br> The <code class="language-plaintext highlighter-rouge">mets/structMap/@TYPE</code> attribute must take the value “PHYSICAL” from the vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStructMapType">Structural map typing</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP82"></a><strong>CSIP82</strong>
</td>
      <td>
<strong>Name of the structural description</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']</code> <br> The <code class="language-plaintext highlighter-rouge">mets/structMap/@LABEL</code> attribute value is set to “CSIP” from the vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyStructMapLabel">Structural map label</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP83"></a><strong>CSIP83</strong>
</td>
      <td>
<strong>Structural description identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/@ID</code> <br> An <code class="language-plaintext highlighter-rouge">xml:id</code> identifier for the structural description (structMap) used for internal package references. It must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP84"></a><strong>CSIP84</strong>
</td>
      <td>
<strong>Main structural division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div</code> <br> The structural map comprises a single division.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP85"></a><strong>CSIP85</strong>
</td>
      <td>
<strong>Main structural division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP86"></a><strong>CSIP86</strong>
</td>
      <td>
<strong>Main structural division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/@LABEL</code> <br> The package’s top-level structural division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element’s <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute value must be identical to the package identifier, i.e. the same value as the <code class="language-plaintext highlighter-rouge">mets/@OBJID</code> attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP88"></a><strong>CSIP88</strong>
</td>
      <td>
<strong>Metadata division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']</code> <br> The metadata referenced in the administrative and/or descriptive metadata section is described in the structural map with one sub division. <br> When the transfer consists of only administrative and/or descriptive metadata this is the only sub division that occurs.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP89"></a><strong>CSIP89</strong>
</td>
      <td>
<strong>Metadata division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP90"></a><strong>CSIP90</strong>
</td>
      <td>
<strong>Metadata division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']</code> <br> The metadata division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element’s <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute value must be “Metadata”. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP91"></a><strong>CSIP91</strong>
</td>
      <td>
<strong>Metadata division administrative metadata referencing</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']/@ADMID</code> <br> When there is administrative metadata and the amdSec is present, all administrative metadata MUST be referenced via the administrative sections different identifiers. <br> All of the <code class="language-plaintext highlighter-rouge">&lt;amdSec&gt;</code> identifiers are listed in a single <code class="language-plaintext highlighter-rouge">@ADMID</code> using spaces as delimiters.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP92"></a><strong>CSIP92</strong>
</td>
      <td>
<strong>Metadata division descriptive metadata referencing</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Metadata']/@DMDID</code> <br> When there are descriptive metadata and one or more dmdSec is present, all descriptive metadata MUST be referenced via the descriptive section identifiers. <br> Every <code class="language-plaintext highlighter-rouge">&lt;dmdSec&gt;</code> identifier is listed in a single <code class="language-plaintext highlighter-rouge">@DMDID</code> attribute using spaces as delimiters.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP93"></a><strong>CSIP93</strong>
</td>
      <td>
<strong>Documentation division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']</code> <br> The documentation referenced in the file section file groups is described in the structural map with one sub division.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP94"></a><strong>CSIP94</strong>
</td>
      <td>
<strong>Documentation division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP95"></a><strong>CSIP95</strong>
</td>
      <td>
<strong>Documentation division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']</code> <br> The documentation division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element in the package uses the value “Documentation” from the vocabulary as the value for the <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP96"></a><strong>CSIP96</strong>
</td>
      <td>
<strong>Documentation file referencing</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']/fptr</code> <br> All file groups containing documentation described in the package are referenced via the relevant file group identifiers. There MUST be one file group reference per <code class="language-plaintext highlighter-rouge">&lt;fptr&gt;</code> element.</td>
      <td>
<strong>0..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP116"></a><strong>CSIP116</strong>
</td>
      <td>
<strong>Documentation file group reference pointer</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Documentation']/fptr/@FILEID</code> <br> A reference, by ID, to the “Documentation” file group. <br> Related to the requirements CSIP60 which describes the “Documentation” file group and CSIP65 which describes the file group identifier.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP97"></a><strong>CSIP97</strong>
</td>
      <td>
<strong>Schema division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']</code> <br> The schemas referenced in the file section file groups are described in the structural map within a single sub-division.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP98"></a><strong>CSIP98</strong>
</td>
      <td>
<strong>Schema division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP99"></a><strong>CSIP99</strong>
</td>
      <td>
<strong>Schema division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']</code> <br> The schema division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element’s <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute has the value “Schemas” from the vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP100"></a><strong>CSIP100</strong>
</td>
      <td>
<strong>Schema file reference</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']/fptr</code> <br> All file groups containing schemas described in the package are referenced via the relevant file group identifiers. One file group reference per fptr-element</td>
      <td>
<strong>0..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP118"></a><strong>CSIP118</strong>
</td>
      <td>
<strong>Schema file group reference</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Schemas']/fptr/@FILEID</code> <br> The pointer to the identifier for the “Schema” file group. <br> Related to the requirements CSIP113 which describes the “Schema” file group and CSIP65 which describes the file group identifier.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP101"></a><strong>CSIP101</strong>
</td>
      <td>
<strong>Content division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']</code> <br> When no representations are present the content referenced in the file section file group with <code class="language-plaintext highlighter-rouge">@USE</code> attribute value “Representations” is described in the structural map as a single sub division.</td>
      <td>
<strong>0..1</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP102"></a><strong>CSIP102</strong>
</td>
      <td>
<strong>Content division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP103"></a><strong>CSIP103</strong>
</td>
      <td>
<strong>Content division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']</code> <br> The package’s content division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element must have the <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute value “Representations”, taken from the vocabulary. <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP104"></a><strong>CSIP104</strong>
</td>
      <td>
<strong>Content division file references</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']/fptr</code> <br> All file groups containing content described in the package are referenced via the relevant file group identifiers. One file group reference per fptr-element.</td>
      <td>
<strong>0..n</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP119"></a><strong>CSIP119</strong>
</td>
      <td>
<strong>Content division file group references</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div[@LABEL='Representations']/fptr/@FILEID</code> <br> The pointer to the identifier for the “Representations” file group. <br> Related to the requirements CSIP114 which describes the “Representations” file group and CSIP65 which describes the file group identifier.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP105"></a><strong>CSIP105</strong>
</td>
      <td>
<strong>Representation division</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div</code> <br> When a package consists of multiple representations, each described by a representation level METS.xml document, there is a discrete representation div element for each representation. <br> Each representation div references the representation level METS.xml document, documenting the structure of the package and its constituent representations.</td>
      <td>
<strong>0..n</strong> <br> SHOULD</td>
    </tr>
    <tr>
      <td>
<a name="CSIP106"></a><strong>CSIP106</strong>
</td>
      <td>
<strong>Representations division identifier</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div/@ID</code> <br> Mandatory, <code class="language-plaintext highlighter-rouge">xml:id</code> identifier must be unique within the package.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP107"></a><strong>CSIP107</strong>
</td>
      <td>
<strong>Representations division label</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div/@LABEL</code> <br> The package’s representation division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> element <code class="language-plaintext highlighter-rouge">@LABEL</code> attribute value must be the path to the representation level METS document. <br> This requirement gives the same value to be used as the requirement named “File group identifier” (CSIP64) <br> <strong>See also:</strong> <a href="#VocabularyFileGrpAndStructMapDivisionLabel">File group names</a>
</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP108"></a><strong>CSIP108</strong>
</td>
      <td>
<strong>Representations division file referencing</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div/mptr/@xlink:title</code> <br> The file group containing the files described in the package are referenced via the relevant file group identifier. <br> Related to the requirements CSIP114 which describes the “Representations” file group and CSIP65 which describes the file group identifier.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP109"></a><strong>CSIP109</strong>
</td>
      <td>
<strong>Representation METS pointer</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap[@LABEL='CSIP']/div/div/mptr</code> <br> The division <code class="language-plaintext highlighter-rouge">&lt;div&gt;</code> of the specific representation includes one occurrence of the METS pointer <code class="language-plaintext highlighter-rouge">&lt;mptr&gt;</code> element, pointing to the appropriate representation METS file.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP110"></a><strong>CSIP110</strong>
</td>
      <td>
<strong>Resource location</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap/div/div/mptr/@xlink:href</code> <br> The actual location of the resource. We  recommend recording a URL type filepath within this attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP111"></a><strong>CSIP111</strong>
</td>
      <td>
<strong>Type of link</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap/div/div/mptr[@xlink:type='simple']</code> <br> Attribute used with the value “simple”. Value list is maintained by the xlink standard.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="CSIP112"></a><strong>CSIP112</strong>
</td>
      <td>
<strong>Type of locator</strong> <br> <code class="language-plaintext highlighter-rouge">mets/structMap/div/div/mptr[@LOCTYPE='URL']</code> <br> The locator type is always used with the value “URL” from the vocabulary in the attribute.</td>
      <td>
<strong>1..1</strong> <br> MUST</td>
    </tr>
    <tr>
      <td>
<a name="REF_METS_1"></a><strong>REF_METS_1</strong>
</td>
      <td>
<strong>structLink</strong> <br>  <br> Section not defined or used in CSIP, additional own uses may occur. <br> Information regarding the structural links is found in the  <a href="http://www.loc.gov/standards/mets/METSPrimer.pdf">METS Primer</a>
</td>
      <td>
<br> MAY</td>
    </tr>
    <tr>
      <td>
<a name="REF_METS_2"></a><strong>REF_METS_2</strong>
</td>
      <td>
<strong>behaviorSec</strong> <br>  <br> Section not defined or used in CSIP, additional own uses may occur. <br> Information regarding the behaviour section is found in the  <a href="http://www.loc.gov/standards/mets/METSPrimer.pdf">METS Primer</a>
</td>
      <td>
<br> MAY</td>
    </tr>
  </tbody>
</table>

<h1 id="postface">Postface</h1>

<h2 id="i-authors">I. Authors</h2>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Organisation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Sven Schlarb</td>
      <td>Austrian Institute of Technology</td>
    </tr>
    <tr>
      <td>Anders Bo Nielsen</td>
      <td>Danish National Archives</td>
    </tr>
    <tr>
      <td>Phillip Mike Tømmerholt</td>
      <td>Danish National Archives</td>
    </tr>
    <tr>
      <td>Kuldar Aas</td>
      <td>Estonian National Archives</td>
    </tr>
    <tr>
      <td>Koit Saarevet</td>
      <td>Estonian National Archives</td>
    </tr>
    <tr>
      <td>Jaime Kaminski</td>
      <td>Highbury IVS</td>
    </tr>
    <tr>
      <td>Miguel Ferreira</td>
      <td>Keep Solutions</td>
    </tr>
    <tr>
      <td>Helder Silva</td>
      <td>Keep Solutions</td>
    </tr>
    <tr>
      <td>Carl Wilson</td>
      <td>Open Preservation Foundation</td>
    </tr>
    <tr>
      <td>Karin Bredenberg</td>
      <td>Kommunalförbundet Sydarkivera</td>
    </tr>
  </tbody>
</table>

<h3 id="ii-contributors-to-previous-version">I.I. Contributors to previous version</h3>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Organisation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Karin Bredenberg</td>
      <td>Kommunalförbundet Sydarkivera</td>
    </tr>
    <tr>
      <td>Björn Skog</td>
      <td>ES Solutions</td>
    </tr>
    <tr>
      <td>Anders Bo Nielsen</td>
      <td>Danish National Archives</td>
    </tr>
    <tr>
      <td>Kathrine Hougaard Edsen Johansen</td>
      <td>Danish National Archives</td>
    </tr>
    <tr>
      <td>Alex Thirifays</td>
      <td>Danish National Archives &amp; Magenta ApS</td>
    </tr>
    <tr>
      <td>Sven Schlarb</td>
      <td>Austrian Institute of Technology</td>
    </tr>
    <tr>
      <td>Andrew Wilson</td>
      <td>University of Portsmouth &amp; University of Brighton</td>
    </tr>
    <tr>
      <td>Tarvo Kärberg</td>
      <td>National Archives of Estonia</td>
    </tr>
    <tr>
      <td>Kuldar Aas</td>
      <td>National Archives of Estonia</td>
    </tr>
    <tr>
      <td>Luis Faria</td>
      <td>Keep Solutions</td>
    </tr>
    <tr>
      <td>Helder Silva</td>
      <td>Keep Solutions</td>
    </tr>
    <tr>
      <td>Miguel Ferreira</td>
      <td>Keep Solutions</td>
    </tr>
    <tr>
      <td>Carl Wilson</td>
      <td>Open Preservation Foundation</td>
    </tr>
  </tbody>
</table>

<h2 id="ii-revision-history">II. Revision History</h2>

<table>
  <thead>
    <tr>
      <th>Revision</th>
      <th>Date</th>
      <th>Authors(s)</th>
      <th>Organisation</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0.1</td>
      <td>17.02.2014</td>
      <td>Björn Skog</td>
      <td>ESS</td>
      <td>First version.</td>
    </tr>
    <tr>
      <td>0.2</td>
      <td>21.02.2014</td>
      <td>Karin Bredenberg</td>
      <td>ESS</td>
      <td>Updating content.</td>
    </tr>
    <tr>
      <td>0.3</td>
      <td>24.02.2014</td>
      <td>Björn Skog</td>
      <td>ESS</td>
      <td>Updating content.</td>
    </tr>
    <tr>
      <td>0.4</td>
      <td>24.10.2014</td>
      <td>Tarvo Kärberg</td>
      <td>NAE</td>
      <td>Updating content.</td>
    </tr>
    <tr>
      <td>0.41</td>
      <td>05.11.2014</td>
      <td>Tarvo Kärberg</td>
      <td>NAE</td>
      <td>Adding content from Anders Bo Nielsen.</td>
    </tr>
    <tr>
      <td>0.42</td>
      <td>08.12.2014</td>
      <td>Tarvo Kärberg</td>
      <td>NAE</td>
      <td>Updating content.</td>
    </tr>
    <tr>
      <td>0.43</td>
      <td>19.12.2014</td>
      <td>Tarvo Kärberg</td>
      <td>NAE</td>
      <td>Updating content.</td>
    </tr>
    <tr>
      <td>0.5</td>
      <td>26.01.2015</td>
      <td>Kathrine Hougaard Edsen</td>
      <td>DNA</td>
      <td>Updating content.</td>
    </tr>
    <tr>
      <td>0.6</td>
      <td>11.02.2015</td>
      <td>Tarvo Kärberg</td>
      <td>NAE</td>
      <td>Rearranging content.</td>
    </tr>
    <tr>
      <td>0.7</td>
      <td>31.05.2015</td>
      <td>Kathrine Hougaard Edsen</td>
      <td>DNA</td>
      <td>Significant changes suggested</td>
    </tr>
    <tr>
      <td>0.8</td>
      <td>27.07.2015</td>
      <td>Tarvo Kärberg</td>
      <td>NAE</td>
      <td>Merging content</td>
    </tr>
    <tr>
      <td>0.9</td>
      <td>05.08.2015</td>
      <td>Andrew Wilson</td>
      <td>UPHEC</td>
      <td>Updating content</td>
    </tr>
    <tr>
      <td>0.10</td>
      <td>07.10.2015</td>
      <td>Kuldar Aas</td>
      <td>NAE</td>
      <td>Major update to include additional details</td>
    </tr>
    <tr>
      <td>0.11</td>
      <td>30.11.2015</td>
      <td>Kuldar Aas</td>
      <td>NAE</td>
      <td>Intermediate update to include outcomes and decisions from Common Specification meetings</td>
    </tr>
    <tr>
      <td>0.12</td>
      <td>08.12.2015</td>
      <td>Kuldar Aas</td>
      <td>NAE</td>
      <td>Update on the implementation, include comments from Sven, Jan (AIT) and Andrew (UPHEC)</td>
    </tr>
    <tr>
      <td>0.13</td>
      <td>05.01.2016</td>
      <td>Kuldar Aas, all</td>
      <td>NAE, all</td>
      <td>Update to include additional comments from E-ARK WPLs and Common Specification group members version sent for external review</td>
    </tr>
    <tr>
      <td>0.14</td>
      <td>04.07.2016</td>
      <td>Kuldar Aas</td>
      <td>NAE</td>
      <td>Updated structure -&gt; basis for addressing review comments and required updates</td>
    </tr>
    <tr>
      <td>0.15</td>
      <td>26.08.2016</td>
      <td>Kuldar Aas</td>
      <td>NAE</td>
      <td>Adding available contributions to individual Sections</td>
    </tr>
    <tr>
      <td>0.16</td>
      <td>05.12.2016</td>
      <td>Andrew Wilson, Kuldar Aas</td>
      <td>UoB, NAE</td>
      <td>Major update. Added section on PREMIS. Revision of tables describing use of METS. General text revisions arising from CS meetings. Updates to requirements.</td>
    </tr>
    <tr>
      <td>0.17</td>
      <td>16.12.2016</td>
      <td>All</td>
      <td>All</td>
      <td>Final discussions, changes and proofreading before delivering the CS to public comment.</td>
    </tr>
    <tr>
      <td>1.0</td>
      <td>31.01.2017</td>
      <td>Kuldar Aas</td>
      <td>NAE</td>
      <td>Final small editorial additions</td>
    </tr>
    <tr>
      <td>1.1</td>
      <td>14.05.2018</td>
      <td>Kuldar Aas (editor), DILCIS Board</td>
      <td>NAE</td>
      <td>Limited proofreading and updates throughout the document. Updates in terminology. Updates in use of METS, ID and referencing section. Improved (more consistent) examples in METS section.</td>
    </tr>
    <tr>
      <td>2.0-DRAFT</td>
      <td>28.11.2018</td>
      <td>DILCIS Board, E-ARK4ALL</td>
      <td>DILCIS Board</td>
      <td>Specification updated and released for open review.</td>
    </tr>
    <tr>
      <td>2.0.0</td>
      <td>31.05.2019</td>
      <td>DILCIS Board, E-ARK4ALL</td>
      <td>DILCIS Board</td>
      <td>Specification updated after open review.</td>
    </tr>
    <tr>
      <td>2.0.1</td>
      <td>09.09.2019</td>
      <td>Karin Bredenberg, C. Wilson, &amp; H. Silva</td>
      <td>NAS, OPF &amp; KEEPS</td>
      <td>Correction <a href="https://github.com/LABEL" class="user-mention">@LABEL</a> and <a href="https://github.com/USE" class="user-mention">@USE</a> attributes, typos, layout and PDF formatting.</td>
    </tr>
    <tr>
      <td>2.0.2</td>
      <td>28.10.2019</td>
      <td>Karin Bredenberg</td>
      <td>SYD</td>
      <td>Fixed schema paths.</td>
    </tr>
    <tr>
      <td>2.0.3</td>
      <td>08.01.2020</td>
      <td>Karin Bredenberg, C.Wilson</td>
      <td>SYD &amp; OPF</td>
      <td>Fixed error in value list note type.</td>
    </tr>
    <tr>
      <td>2.0.4</td>
      <td>12.06.2020</td>
      <td>K. Bredenberg, C.Wilson &amp; J. Kaminski</td>
      <td>SYD, OPF &amp; HIGH</td>
      <td>Update in example ID:s, preface text and output display update</td>
    </tr>
  </tbody>
</table>

<h2 id="iii-acknowledgements">III. Acknowledgements</h2>

<p>The Common Specification for Information Packages was first developed within the E-ARK project in 2014 – 2017. E-ARK was an EC-funded pilot action project in the Competiveness and Innovation Programme 2007- 2013, Grant Agreement no. 620998 under the Policy Support Programme.</p>

<p>We would like to thank the National Archives of Sweden and Karin Bredenberg for their support and the availability of the Swedish national Common Specifications, upon which most of this document has been built.</p>

<p>The authors of this deliverable would like to thank all national archives, tool developers and other stakeholders who provided valuable knowledge about their requirements for information packages and feedback to this specification!</p>

<h2 id="iv-contact--feedback">IV. Contact &amp; Feedback</h2>

<p>The Common Specification for Information Packages is maintained by the Digital Information LifeCycle
Interoperability Standard Board (DILCIS Board). For further information about the DILCIS Board or feedback
on the current document please consult the website <a href="http://www.dilcis.eu/">http://www.dilcis.eu/</a> or contact us at
<a href="mailto:info@dilcis.eu">info@dilcis.eu</a>.</p>

  </div>
      <!-- FOOTER -->
    <footer id="footer" class="wrap footer">
    	<section class="copyright">
    		<div class="container">
    			<div class="row">
    				<div class="col-md-12 copyright ">
              <div class="custom">
    	          <h3>
<img style="float: left;" src="/img/Logo_DILCIS_one_color-01.png" alt="DILCIS logo" width="234" height="69"><img style="float: right;" src="/img/DLM-Forum-lofo.png" alt="DLM-Forum Logo" width="95" height="72">
</h3>
                <h5 style="text-align: center;"> </h5>
                <h5 style="text-align: center;">This site is maintained by the Digital Information LifeCycle Interoperability Standards Board. </h5>
                <h6 style="text-align: center;">© DILCIS Board, 2019</h6>
              </div>
              <small>
                <a href="http://twitter.github.io/bootstrap/" title="Bootstrap by Twitter" target="_blank">Bootstrap</a> is a front-end framework of Twitter, Inc. Code licensed under <a href="https://github.com/twbs/bootstrap/blob/master/LICENSE" title="MIT License" target="_blank">MIT License.</a>
              </small>
    				</div>
					</div>
    		</div>
    	</section>
    </footer>
    <!-- //FOOTER -->

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>

</body>
</html>
© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About