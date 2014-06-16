<html><head>
      <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
   
      <style>
      body {font-family: Helvetica, Arial, sans-serif;font-size: 12px;
}


      a {color:#000099;
}

a:visited {color:#840084;
}

a:active {color:#000099;
}

a:hover {color:#000033;
}

hr {border-style: solid;border-width: 1px 0px 0px 0px;height: 1px;width: 100%;color: #000000;
}

p {margin-left: 5px;
}

td {font-family: Helvetica, Arial, sans-serif;font-size: 12px;
}

.title {color:#990000;font-size:24px;padding:2px 0px 2px 0px;margin:10px 0px 0px 5px;vertical-align: middle;
}

.sectiontitle {color:#990000;font-size:16px;font-weight: bold;width:100%;padding:2px 0px 2px 5px;margin: 15px 0px 0px 0px;
}

.headertitle {font-weight:bold;padding: 3px 5px 3px 5px;
}

.helptopic {font-weight:bold;color:#990000;
}

.helptext {margin-left: 5px;font-family: monospace; white-space: pre;font-size: 13px;
}

.subheader {background-color: #E7EBF7;width: 100%;
}

.subheader-left {padding: 3px 5px 3px 5px;
}

.subheader-right {text-align: right;padding: 3px 5px 3px 5px;
}

.footerlinktitle {margin: 15px 0px 0px 5px;color:#990000;font-size: 16px;
}

.footerlink {padding: 3px 5px 3px 15px;
}

.topiclinks {margin: 5px 0px 0px 5px;
}

a.topiclink {padding-right: 10px;
}

.class-details {border-width: 0px 0px 0px 0px;margin: 0px 0px 0px 5px;
}

.class-detail-label {font-weight: bold;padding: 0px 10px 0px 0px;spacing: 0px 0px 0px 0px;
}

.summary-list .m-help {white-space: nowrap;
}

.summary-list {margin: 0px 15px 0px 15px;
}

.summary-list .summary-item .name  {border-width: 0px 0px 1px 0px;border-style: solid;border-color:#E7EBF7;padding: 2px 15px 2px 5px;
}

.summary-list .summary-item .m-help {border-width: 0px 0px 1px 0px;border-style: solid;border-color:#E7EBF7;padding: 2px 5px 2px 5px;width: 95%;white-space: normal;
}

.summary-list .summary-item .attributes {border-width: 0px 0px 1px 0px;border-style: solid;border-color:#E7EBF7;padding: 2px 15px 2px 5px;white-space: nowrap;
}
  
      </style>
      
      <title>MATLAB File Help: nanfillts</title>
   </head>
   <body>
      <!--Single-page help-->
      <div class="title">nanfillts</div>

  <span class="helptopic">nanfillts</span> Fill NaNs in the time series with the previous valid observation
 
    <span class="helptopic">nanfillts</span>(TSPANEL) TSPANEL should be a numeric matrix (or a vector) 
                       where each series is a column with the oldest 
                       observations in the first row (element) and the 
                       most recent ones in the last row (element).
 
    <span class="helptopic">nanfillts</span>(..., NOTRAIL) To avoid extrapolation of the last value of a 
                            time series till the end of the panel, set 
                            NOTRAIL to true (1). By default is false (0).
 
 
    TSPANEL = <span class="helptopic">nanfillts</span>(...) Returns the same matrix with filled NaNs.
 
    NOTE: leading NaNs are left untouched.
 
 
  Example:
 
    % Input data       % Simple call       % No trailing
                       nanfillts(ts)       nanfillts(ts,1)
     ts =              ans =               ans = 
         10  NaN            10  NaN             10  NaN
        NaN  NaN            10  NaN             10  NaN
        NaN    1            10    1             10    1
          9    2             9    2              9    2
        NaN  NaN             9    2            NaN  NaN
 
  Additional features:
  - <a href="matlab: web('https://github.com/okomarov/nanfillts','-browser')">GITHUB/nanfillts page</a></pre></div><!--after help --><!--seeAlso--><div class="footerlinktitle">See also</div><div class="footerlink"> <a href="matlab:helpPopup interp1q">interp1q</a>
</div>
   
</body></html>