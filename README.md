# oxygenxml.icu4j.i18n
An Oxygen XML Editor plugin which provides the entire ICU4j JAR library used for sorting and collations with XSLT processors.
For example when using the xsl:sort element:

            <xsl:for-each select="/*/*">
                <xsl:sort select="." collation="http://www.w3.org/2013/collation/UCA?lang=ta"/> 
                <xsl:copy-of select="."/>
            </xsl:for-each>
            
the Saxon 9 processor will use this additional library to better sort texts in exotic languages.

In order to install the plugin go to the Oxygen Help menu->"Install new add-ons" paste the link:

https://raw.githubusercontent.com/oxygenxml/oxygenxml.icu4j.i18n/master/addon.xml

and follow the procedure.
