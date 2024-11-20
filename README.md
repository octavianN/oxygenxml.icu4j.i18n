# HTMLParser JAR Library

This Oxygen XML Editor plugin provides the entire HTMLParser JAR library used for XSLT processors.

For example, the Saxon XSLT processor has an *saxon:parse-html* function that need the html parser library in the class path:

             <xsl:template name="xsl:initial-template">
                 <xsl:sequence select="saxon:parse-html('&lt;html&gt;&lt;p&gt;test&lt;/p&gt;&lt;/html&gt;')"/>
             </xsl:template>
            
How to install
--------------
1. In Oxygen, go to **Help->Install new add-ons** to open an add-on selection dialog box.
2. Enter or paste https://raw.githubusercontent.com/octaviann/oxygenxml.icu4j.i18n/html-parser/addon.xml in the **Show add-ons from** field.
3. Select the **Contribute HTMLParser Library** add-on and click Next.
4. Read the end-user license agreement. Then select the **I accept all terms of the end-user license agreement** option and click **Finish**.
5. Restart the application.

Copyright and License
---------------------
Copyright 2018 Syncro Soft SRL.

This project is licensed under [Apache License 2.0](https://github.com/oxygenxml/oxygenxml.icu4j.i18n/blob/html-parser/LICENSE)
