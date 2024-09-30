<?xml version="1.0"?>
<flowgorithm fileversion="4.2">
    <attributes>
        <attribute name="name" value="Guessing Game 1-5"/>
        <attribute name="authors" value="Payton"/>
        <attribute name="about" value=""/>
        <attribute name="saved" value="2024-09-29 10:24:22 PM"/>
        <attribute name="created" value="UGF5dG9uO1BBWVRPTi1QQzsyMDI0LTA5LTI5OzA5OjUyOjA5IFBNOzI1OTk="/>
        <attribute name="edited" value="UGF5dG9uO1BBWVRPTi1QQzsyMDI0LTA5LTI5OzEwOjI0OjIyIFBNOzE7MjY5Mw=="/>
    </attributes>
    <function name="Main" type="None" variable="">
        <parameters/>
        <body>
            <declare name="RandomNumber" type="Integer" array="False" size=""/>
            <declare name="Guess" type="Integer" array="False" size=""/>
            <assign variable="RandomNumber" expression="Random(5)"/>
            <output expression="&quot;Enter a number between 1 and 5&quot;" newline="True"/>
            <input variable="Guess"/>
            <while expression="Guess &lt;&gt; RandomNumber">
                <if expression="Guess &lt; RandomNumber">
                    <then>
                        <output expression="&quot;To Low&quot;" newline="True"/>
                    </then>
                    <else>
                        <if expression="Guess &gt; RandomNumber">
                            <then>
                                <output expression="&quot;To High&quot;" newline="True"/>
                            </then>
                            <else/>
                        </if>
                    </else>
                </if>
                <output expression="&quot;Enter a number between 1 and 5&quot;" newline="True"/>
                <input variable="Guess"/>
            </while>
            <output expression="&quot;Correct! Play again?&quot;" newline="True"/>
        </body>
    </function>
</flowgorithm>
