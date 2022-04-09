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
                        <name>EventTitle</name>
                        <description>name of the event</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>EventDescription</name>
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
                        <name>Event-info1</name>
                        <description>event info 1 (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>Event-info2</name>
                        <description>event info 2 (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>Event-info3</name>
                        <description>event info 3 (optional)</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                </inputs>
            </idm>
        </component>

Also, you should add in "\Datalet-Ecosystem-Provider\deep-components\locales\controllet_ln.js" the proper translation for the controllet (english and italian):

ENGLISH:

        //logtimeline english lan
        ln["timeline_en"] = "logtimeline-datalet";
        
        ln["Start Date"] = "StartDate";
        ln["StartDatedescription_en"] = "Event Start Date";
        
        ln["End Date"] = "EndDate";
        ln["EndDatedescription_en"] = "Event End Date";
        
        ln["Event Title"] = "EventTitle";
        ln["EventTitledescription_en"] = "Name of the event";
        
        ln["Event Description"] = "EventDescription";
        ln["EventDescriptiondescription_en"] = "Event Description";
        
        ln["MediaUrl"] = "MediaUrl";
        ln["MediaUrldescription_en"] = "Url of video/image";
        
        ln["Background"] = "Background";
        ln["Backgrounddescription_en"] = "Url of background image";
        
        ln["Start Time"] = "StartTime";
        ln["StartTimedescription_en"] = "Event start time";
        
        ln["Finish Time"] = "FinishTime";
        ln["FinishTimedescription_en"] = "Event end time";
        
        ln["Event info 1"] = "Event-info1";
        ln["EventInfo1description_en"] = "Additional info 1";
        
        ln["Event info 2"] = "Event-info2";
        ln["EventInfo2description_en"] = "Additional info 2";
        
        ln["Event info 3"] = "Event-info3";
        ln["EventInfo3description_en"] = "Additional info 3";
         

ITALIAN:

        //logtimeline italian lan
        ln["timeline_it"] = "logtimeline-datalet";
        
        ln["Data di inizio"] = "StartDate";
        ln["StartDatedescription_it"] = "Data iniziale dell'evento";
        
        ln["Data di fine"] = "EndDate";
        ln["EndDatedescription_it"] = "Data di fine dell'evento";
        
        ln["Titolo evento"] = "EventTitle";
        ln["EventTitledescription_it"] = "Nome dell'evento";
        
        ln["Descrizione"] = "EventDescription";
        ln["EventDescriptiondescription_it"] = "Descrizione dell'evento";
        
        ln["MediaUrl"] = "MediaUrl";
        ln["MediaUrldescription_it"] = "Url dell'immagine o video";
        
        ln["Immagine di sfondo"] = "Background";
        ln["Backgrounddescription_it"] = "Url dell'immagine di sfondo";
        
        ln["Orario di inizio"] = "StartTime";
        ln["StartTimedescription_it"] = "Orario di inzio dell'evento";
        
        ln["Orario di fine"] = "FinishTime";
        ln["FinishTimedescription_it"] = "Orario di fine dell'evento";
        
        ln["Informazione evento 1"] = "Event-info1";
        ln["EventInfo1description_it"] = "Informazione aggiuntiva dell'evento";
        
        ln["Informazione evento 2"] = "Event-info2";
        ln["EventInfo2description_it"] = "Informazione aggiuntiva dell'evento";
        
        ln["Informazione evento 3"] = "Event-info3";
        ln["EventInfo3description_it"] = "Informazione aggiuntiva dell'evento";        
