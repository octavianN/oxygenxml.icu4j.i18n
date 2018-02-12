# ICU4j JAR Library

This Oxygen XML Editor plugin provides the entire ICU4j JAR library used for sorting and collations with XSLT processors.

For example, the Saxon 9 XSLT processor has an *xsl:sort* element that can be used to sort elements based on their text content:

            <xsl:for-each select="/*/*">
                <xsl:sort select="." collation="http://www.w3.org/2013/collation/UCA?lang=ta"/> 
                <xsl:copy-of select="."/>
            </xsl:for-each>
            
If the XML elements contain texts in exotic languages, Saxon needs a more powerful sort algorithm and the ICU4J library provides this extra support.

How to install
--------------
1. In Oxygen, go to **Help->Install new add-ons** to open an add-on selection dialog box.
2. Enter or paste https://raw.githubusercontent.com/oxygenxml/oxygenxml.icu4j.i18n/master/addon.xml in the **Show add-ons from** field.
3. Select the **Translation Package Builder** add-on and click Next.
4. Select the **I accept all terms of the end user license agreement** option and click **Finish**.
5. Restart the application.
