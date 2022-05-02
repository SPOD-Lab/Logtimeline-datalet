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
                        <description>LOGTIMELINEStartDateDescription</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEndDate</name>
                        <description>LOGTIMELINEEndDateDescription</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventTitle</name>
                        <description>LOGTIMELINEEventTitleDescription</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventDescription</name>
                        <description>LOGTIMELINEEventDescriptionDescription</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEMediaUrl</name>
                        <description>LOGTIMELINEMediaUrlDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEBackground</name>
                        <description>LOGTIMELINEBackgroundDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEStartTime</name>
                        <description>LOGTIMELINEStartTimeDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEFinishTime</name>
                        <description>LOGTIMELINEFinishTimeDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventInfo1</name>
                        <description>LOGTIMELINEEventInfo1Description</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventInfo2</name>
                        <description>LOGTIMELINEEventInfo2Description</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventInfo3</name>
                        <description>LOGTIMELINEEventInfo3Description</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINELink</name>
                        <description>LOGTIMELINELinkDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <layouts>
                        <input>
                            <name>date-reading</name>
                            <description>date-readingDescription</description>
                            <type>LIST</type>
                            <selection>1</selection>
                            <list>
                                <item>Std</item>
                                <item>Alt</item>
                            </list>
                        </input>
                        <input>
                            <name>timenav-position</name>
                            <description>timenav-positionDescription</description>
                            <type>LIST</type>
                            <selection>1</selection>
                            <list>
                                <item>Bottom</item>
                                <item>Top</item>
                            </list>
                        </input>
                        <input>
                            <name>lang-timeline</name>
                            <description>lang-timelineDescription</description>
                            <type>LIST</type>
                            <selection>1</selection>
                            <list>
                                <item>en</item>
                                <item>it</item>
                                <item>fr</item>
                                <item>de</item>
                                <item>es</item>
                                <item>cn</item>
                                <item>ja</item>
                            </list>
                        </input>
                        <input>
                            <name>slides-order</name>
                            <description>slides-orderDescription</description>
                            <type>LIST</type>
                            <selection>?</selection>
                            <list>
                                <item>start</item>
                                <item>end</item>
                            </list>
                        </input>
                        <input>
                            <name>LOGTIMELINETheme</name>
                            <description>LOGTIMELINEThemeDescription</description>
                            <type>LIST</type>
                            <selection>?</selection>
                            <list>
                                <item>light</item>
                                <item>dark</item>
                            </list>
                        </input>
                        <input>
                            <name>hash_bookmark</name>
                            <description>hash_bookmarkDescription</description>
                            <type>LIST</type>
                            <selection>?</selection>
                            <list>
                                <item>off</item>
                                <item>on</item>
                            </list>
                        </input>
                    </layouts>
                </inputs>
            </idm>
        </component>

Also, you should add in "\Datalet-Ecosystem-Provider\deep-components\locales\controllet_ln.js" the proper translation for the controllet (english and italian):

ENGLISH:

	//logtimeline english lan
	ln["logtimeline_en"] = "Log timeline";
	ln["logtimelineDescription_en"] = "The logtimeline-datalet is an interactive visualization of event logs on timeline. The event logs are a basic resource that helps provide information about network traffic and other conditions. The events can have a start date and end date or a single date. You also can add the start time and/or end time details from dataset with only time schedule information. You can add event title, event description and other additional event info. It's possible to freely move and zoom the timeline.";
	ln["LOGTIMELINEStartDate_en"] = "Start date";
	ln["LOGTIMELINEStartDateDescription_en"] = "Start date of the event. The logtimeline-datalet supports most of timestamp formats written in log files. For example: the format “yyyy-MM-d’T’HH:mm:ss.SSSZ” (sample value: 2001-07-04T12:08:56.235-0700); the format “yyyyy.MMMMM.dd GGG hh:mm aaa” (sample value: 02001.July.04 AD 12:08:56 -0700); the format “yyyy.MM.dd G ‘at’ HH:mm:ss” (sample value: 2001.07.04 at 12:08:56 PDT).";
	ln["LOGTIMELINEEndDate_en"] = "End date";
	ln["LOGTIMELINEEndDateDescription_en"] = "The end date of the event (see start date). You can use the same information of “Start Date” if the dataset has punctual events.";
	ln["LOGTIMELINEEventTitle_en"] = "Event name";
	ln["LOGTIMELINEEventTitleDescription_en"] = "Event name";
	ln["LOGTIMELINEEventDescription_en"] = "Event description";
	ln["LOGTIMELINEEventDescriptionDescription_en"] = "Event description";
	ln["LOGTIMELINEMediaUrl_en"] = "Media url";
	ln["LOGTIMELINEMediaUrlDescription_en"] = "Url of image or video";
	ln["LOGTIMELINEBackground_en"] = "Background";
	ln["LOGTIMELINEBackgroundDescription_en"] = "URL of background image, CSS colours (for example red, aqua etc.), hexadecimal format (for example # 0f9bd1) or a valid CSS managed colour keyword.";
	ln["LOGTIMELINEStartTime_en"] = "Start Time";
	ln["LOGTIMELINEStartTimeDescription_en"] = "Start time of the event. You can add the time schedule in this input or the full timestamp. The logtimeline-datalet supports these schedule formats: “hh:mm”, “hh:mm:ss”, “hh:mm:ss:ms”, “hh:mm:ss aaa” (for example 12:08:56 -0700), “HH:mm:ssZ” (for example 16:53:34Z), “HH:mm:ss a” (for example 11:31:45 AM) and “hh ‘english time’ a, zzzz” (for example 12 o’clock PM, Pacific Daylight Time).";
	ln["LOGTIMELINEFinishTime_en"] = "Finish Time";
	ln["LOGTIMELINEFinishTimeDescription_en"] = "Finish time of the event. (see start time).";
	ln["LOGTIMELINEEventInfo1_en"] = "Event info 1";
	ln["LOGTIMELINEEventInfo1Description_en"] = "Additional event information.";
	ln["LOGTIMELINEEventInfo2_en"] = "Event info 2";
	ln["LOGTIMELINEEventInfo2Description_en"] = "Additional event information.";
	ln["LOGTIMELINEEventInfo3_en"] = "Event info 3";
	ln["LOGTIMELINEEventInfo3Description_en"] = "Additional event information."
	ln["LOGTIMELINELink_en"] = "Link";
	ln["LOGTIMELINELinkDescription_en"] = "Link";
	ln["date-reading_en"] = "Date reading";
	ln["Std_en"] = "Standard";
	ln["Alt_en"] = "Alternative (first the day)";
	ln["date-readingDescription_en"] = 'The logtimeline read the date in standard mode or in alternative mode (first the day): in standard mode it read the month before the day(for example logtimeline read 10-02-2020 as October, 2); in alternative mode it read the day before the month(for example logtimeline read 10-02-2020 as February, 10).';
	ln["timenav-position_en"] = "Timenav position";
	ln["timenav-positionDescription_en"] = "The position of timeline navigation bar";
	ln["Bottom_en"] = "Bottom";
	ln["Top_en"] = "Top";
	ln["lang-timeline_en"] = "Language";
	ln["lang-timelineDescription_en"] = "The timeline language";
	ln["en_en"] = "English";
	ln["it_en"] = "Italian";
	ln["fr_en"] = "French";
	ln["de_en"] = "German";
	ln["es_en"] = "Spanish";
	ln["cn_en"] = "Chinese";
	ln["ja_en"] = "Japan";
	ln["slides-order_en"] = "Slides loading";
	ln["slides-orderDescription_en"] = 'Load timeline on last or on first slide';
	ln["start_en"] = "On first";
	ln["end_en"] = "On last";
	ln["hash_bookmark_en"] = "Hash bookmark";
	ln["hash_bookmarkDescription_en"] = "If set to ON, logtimeline will update the browser URL each time a slide advances, so that you can link directly to specific slides."
	ln["off_en"] = "OFF";
	ln["on_en"] = "ON";
	ln["LOGTIMELINETheme_en"] = "Theme";
	ln["LOGTIMELINEThemeDescription_en"] = "Theme"
	ln["light_en"] = "Light";
	ln["dark_en"] = "Dark";
	
