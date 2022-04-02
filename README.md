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
                        <name>LOGTIMELINEStartDate</name>
                        <description>start date of the event</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEndDate</name>
                        <description>end date of the event</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEHeadline</name>
                        <description>name of the event</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEDescription</name>
                        <description>description of the event</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEMediaUrl</name>
                        <description>url of video/image (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEBackground</name>
                        <description>url of background image (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEStartTime</name>
                        <description>start time of the event (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEFinishTime</name>
                        <description>end time of the event (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventInfo1</name>
                        <description>event info 1 (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventInfo2</name>
                        <description>event info 2 (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventInfo3</name>
                        <description>event info 3 (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                </inputs>
            </idm>
        </component>

Also, you should add in "\Datalet-Ecosystem-Provider\deep-components\locales\controllet_ln.js" the proper translation for the controllet (english and italian):


        //logtimeline english lan
        ln["timeline_en"] = "Logtimeline";
        
        ln["LOGTIMELINEStartDate_en"] = "StartDate";
        ln["LOGTIMELINEStartDatedescription_en"] = "Event Start Date";
        
        ln["LOGTIMELINEEndDate_en"]="EndDate";
        ln["enddatedescription_en"] = "Event End Date";
        
        ln["LOGTIMELINEHeadline_en"] = "Headline";
        ln["LOGTIMELINEHeadlinedescription_en"] = "Name of the event";
        
        ln["LOGTIMELINEDescription_en"] = "Description";
        ln["LOGTIMELINEDescriptiondescription_en"] = "Event Description";
        
        ln["LOGTIMELINEMediaUrl_en"] = "MediaUrl";
        ln["LOGTIMELINEMediaUrldescription_en"] = "Url of video/image";
        
        ln["LOGTIMELINEStartTime_en"] = "StartTime";
        ln["LOGTIMELINEStartTimedescription_en"] = "Event start time";
        
        ln["LOGTIMELINEFinishTime_en"] = "FinishTime";
        ln["LOGTIMELINEFinishTimedescription_en"] = "Event end time";
        
        ln["LOGTIMELINEEventInfo1_en"] = "EventInfo1";
        ln["LOGTIMELINEEventInfo1description_en"] = "Additional info 1";
        
        ln["LOGTIMELINEEventInfo2_en"] = "EventInfo2";
        ln["LOGTIMELINEEventInfo2description_en"] = "Additional info 2";
        
        ln["LOGTIMELINEEventInfo3_en"] = "EventInfo3";
        ln["LOGTIMELINEEventInfo3description_en"] = "Additional info 3";
         
