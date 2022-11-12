/*
Created by Nathan R
Custom table formatting for Dashboard

To use, paste into format data expression
*/

if ($datapoint.Status == "Denied"){
    var color = "#e9acac"
    };
    
if ($datapoint.Status == "Comments Received"){
    var color = "#f2f0c5"
    };    

if ($datapoint.Status == "Approved"){
    var color = "#a0d3a3"
    };
    
if ($datapoint.Status == "Under Review"){
    if (Today() > DateAdd($datapoint.Date_Submitted, 30, 'days')){
        var color = "#f0f0f0"
        };
    };

return {
        cells: {
           Agency: {
            displayText : $datapoint["Agency"],
            textColor: '',
            backgroundColor: color,
            textAlign: 'left',
            iconName: '',
            iconAlign: '',
            iconColor: '',
            iconOutlineColor: ''
        	},
		 Status: {
            displayText : $datapoint["Status"],
            textColor: '',
            backgroundColor: color,
            textAlign: 'left',
            iconName: '',
            iconAlign: '',
            iconColor: '',
            iconOutlineColor: ''
        	},
		 Review_Type: {
            displayText : $datapoint["Review_Type"],
            textColor: '',
            backgroundColor: color,
            textAlign: 'left',
            iconName: '',
            iconAlign: '',
            iconColor: '',
            iconOutlineColor: ''
        	},
		 Date_Submitted: {
            displayText : Text(Date(DefaultValue($datapoint["Date_Submitted"], '')), 'MM/DD/YY') + " (" + DateDiff(Today(), Date($datapoint["Date_Submitted"]), 'days') + " days ago)",
            textColor: '',
            backgroundColor: color,
            textAlign: 'left',
            iconName: '',
            iconAlign: '',
            iconColor: '',
            iconOutlineColor: ''
        	},
           Status_Date_Received: {
            displayText :  Text(Date(DefaultValue($datapoint["Status_Date_Received"], '')), 'MM/DD/YY') +   IIf($datapoint["Status_Date_Received"] == Null, "", (" (" + DateDiff($datapoint["Status_Date_Received"], $datapoint["Date_Submitted"], 'days') + " days after submittal)"))          ,
            textColor: '',
            backgroundColor: color,
            textAlign: 'left',
            iconName: '',
            iconAlign: '',
            iconColor: '',
            iconOutlineColor: ''
        	},
           Project_Name: {
            displayText : $datapoint["Project_Name"],
            textColor: '',
            backgroundColor: color,
            textAlign: 'left',
            iconName: '',
            iconAlign: '',
            iconColor: '',
            iconOutlineColor: ''
        	},
		
        }
      }
