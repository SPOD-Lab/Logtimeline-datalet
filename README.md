# Logtimeline-datalet
Logtimeline-datalet for event-logs visualization in DEEP

Before using this datalet on SPOD, you must add this lines to "\Datalet-Ecosystem-Provider\deep\datalets.xml":

        <!--Logtimeline-->
        <component>
            <name>logtimeline-datalet</name>
            <type>logtimeline</type>
            <idm>
                <inputs>                  
                    <input>
                        <name>StartDate</name>
                        <description>start date of the event</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>EndDate</name>
                        <description>end date of the event</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>Headline</name>
                        <description>name of the event</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>Description</name>
                        <description>description of the event</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>MediaUrl</name>
                        <description>url of video/image (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>Background</name>
                        <description>url of background image (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>StartTime</name>
                        <description>start time of the event (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>FinishTime</name>
                        <description>end time of the event (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>EventInfo1</name>
                        <description>event info 1 (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>EventInfo2</name>
                        <description>event info 2 (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>EventInfo3</name>
                        <description>event info 3 (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                </inputs>
            </idm>
        </component>
