[![N|Solid](https://www.bobit.us/images/bobit-logo.png)](https://bobit37.github.io/Resume/)

# Pagination Helper Task

This project has been created using Maven and TestNG is used for unit test. 
Download or clone the project on your local system after that in the terminal execute following commands.

## Specify project path on the terminal
- cd project path

## to execute all test cases
- mvn -Dtest=PaginationHelperTest test

## to execute specific test case
- mvn -Dtest=PaginationHelperTest#getItemCount test
- mvn -Dtest=PaginationHelperTest#getPageIndex test
- mvn -Dtest=PaginationHelperTest#getPageCount test
- mvn -Dtest=PaginationHelperTest#getPageItemCount test

## without command line
- go to test resources and find runner package, then execute runnertest.xml file


```
<!DOCTYPE html>
<html>


<head>
	<meta charset='utf-8' /> 
	<meta name='description' content='' />
	<meta name='robots' content='noodp, noydir' />
	<meta name='viewport' content='width=device-width, initial-scale=1' />
	<meta id="timeStampFormat" name="timeStampFormat" content='MMM d, yyyy hh:mm:ss a'/>
	
	<link href='https://fonts.googleapis.com/css?family=Source+Sans+Pro:400,600' rel='stylesheet' type='text/css' />
	<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet" />

		<link href='https://cdn.rawgit.com/anshooarora/extentreports-java/b4a58fcfd1e137bd9287244035a7c80d3d73b3af/dist/css/extent.css' type='text/css' rel='stylesheet' />
	
	<title>Automation Test Results</title>

	<style type='text/css'>
	</style>
</head>

	<body class='extent standard default hide-overflow '>
		<div id='theme-selector' alt='Click to toggle theme. To enable by default, use theme configuration.' title='Click to toggle theme. To enable by default, use theme configuration.'>
			<span><i class='material-icons'>desktop_windows</i></span>
		</div>

<nav>
	<div class="nav-wrapper">
		<a href="#!" class="brand-logo blue darken-3">Extent</a>

		<!-- slideout menu -->
		<ul id='slide-out' class='side-nav fixed hide-on-med-and-down'>
			<li class='waves-effect active'><a href='#!' view='test-view' onclick="configureView(0);chartsView('test');"><i class='material-icons'>dashboard</i></a></li>
						<li class='waves-effect'><a href='#!' view='category-view' onclick="configureView(1)"><i class='material-icons'>label_outline</i></a></li>
			<li class='waves-effect'><a href='#!' onclick="configureView(-1);chartsView('dashboard');" view='dashboard-view'><i class='material-icons'>track_changes</i></i></a></li>
		</ul>

		<!-- report name -->
		<span class='report-name'>Automation Test Results</span>
		
		<!-- report headline -->
		<span class='report-headline'></span>

		<!-- nav-right -->
		<ul id='nav-mobile' class='right hide-on-med-and-down nav-right'>
			<li>
                <a href='#!'>
                    <span class='label suite-start-time blue darken-3'>Mar 27, 2021 11:18:13 PM</span>
				</a>
			</li>
			<li>
                <a href='#!'>
                    <span class='label blue darken-3'>3.1.5</span>
				</a>
			</li>
		</ul>
	</div>
</nav>

		<!-- container -->
		<div class='container'>

<div id='test-view' class='view'>
				
	<section id='controls'>
		<div class='controls grey lighten-4'>
			<!-- test toggle -->
			<div class='chip transparent'>
				<a class='dropdown-button tests-toggle' data-activates='tests-toggle' data-constrainwidth='true' data-beloworigin='true' data-hover='true' href='#'>
					<i class='material-icons'>warning</i> Status
				</a>
				<ul id='tests-toggle' class='dropdown-content'>
											<li status='pass'><a href='#!'>Pass <i class='material-icons green-text'>check_circle</i></a></li>
					<li class='divider'></li>
					<li status='clear' clear='true'><a href='#!'>Clear Filters <i class='material-icons'>clear</i></a></li>
				</ul>
			</div>
			<!-- test toggle -->

			<!-- category toggle -->
			<div class='chip transparent'>
				<a class='dropdown-button category-toggle' data-activates='category-toggle' data-constrainwidth='false' data-beloworigin='true' data-hover='true' href='#'>
					<i class='material-icons'>local_offer</i> Category
				</a>
				<ul id='category-toggle' class='dropdown-content'>
					<li><a href='#'>Suite</a></li>
					<li><a href='#'>JavaScriptErrorPageTest</a></li>
					<li><a href='#'>FileDownloadPageTest</a></li>
					<li><a href='#'>DragDropTest</a></li>
					<li><a href='#'>DynamicLoadingPageTest</a></li>
					<li><a href='#'>MouseHoverPageTest</a></li>
					<li><a href='#'>FileUploadPageTest</a></li>
					<li><a href='#'>DynamicContentPageTest</a></li>
					<li><a href='#'>DynamicControlPageTest</a></li>
					<li><a href='#'>CheckBoxTest</a></li>
					<li><a href='#'>JavaScriptAlertPageTest</a></li>
					<li><a href='#'>DropDownPageTest</a></li>
					<li><a href='#'>ContextMenuPageTest</a></li>
					<li><a href='#'>OpenNewTabPageTest</a></li>
					<li><a href='#'>FloatingMenuPageTest</a></li>
					<li><a href='#'>NotificationMessageRenderedPageTest</a></li>
					<li><a href='#'>LoginPageTest</a></li>
					<li><a href='#'>IFramePageTest</a></li>
					<li class='divider'></li>
					<li class='clear'><a href='#!' clear='true'>Clear Filters</a></li>
				</ul>
			</div>
			<!-- category toggle -->

			<!-- clear filters -->
			<div class='chip transparent hide'>
				<a class='' id='clear-filters' alt='Clear Filters' title='Clear Filters'>
					<i class='material-icons'>close</i> Clear
				</a>
			</div>
			<!-- clear filters -->

			<!-- enable dashboard -->
			<div id='toggle-test-view-charts' class='chip transparent'>
				<a class='pink-text' id='enable-dashboard' alt='Enable Dashboard' title='Enable Dashboard'>
					<i class='material-icons'>track_changes</i> Dashboard
				</a>
			</div>
			<!-- enable dashboard -->

			<!-- search -->
			<div class='chip transparent' alt='Search Tests' title='Search Tests'>
				<a href="#" class='search-div'>
					<i class='material-icons'>search</i> Search
				</a>

				<div class='input-field left hide'>
					<input id='search-tests' type='text' class='validate browser-default' placeholder='Search Tests...'>
				</div>
				
			</div>
			<!-- search -->
		</div>
	</section>


<div id='test-view-charts' class='subview-full'>
	<div id='charts-row' class='row nm-v nm-h'>
		<div class='col s12 m6 l6 np-h'>
			<div class='card-panel nm-v'>
				<div class='left panel-name'>Tests</div>
				<div class='chart-box'>
					<canvas id='parent-analysis' width='100' height='80'></canvas>
				</div>
				<div class='block text-small'>
					<span class='tooltipped' data-position='top' data-tooltip='100%'><span class='strong'>26</span> test(s) passed</span>
				</div>
				<div class='block text-small'>
					<span class='strong tooltipped' data-position='top' data-tooltip='0%'>0</span> test(s) failed, <span class='strong tooltipped' data-position='top' data-tooltip='0%'>0</span> others
				</div>
			</div>
		</div>
		
		<div class='col s12 m6 l6 np-h'>
			<div class='card-panel nm-v'>
				<div class='left panel-name'>Steps</div>
				<div class='chart-box'>
					<canvas id='child-analysis' width='100' height='80'></canvas>
				</div>
				<div class='block text-small'>
					<span class='tooltipped' data-position='top' data-tooltip='100%'><span class='strong'>26</span> step(s) passed</span>
				</div>
				<div class='block text-small'>
					<span class='strong tooltipped' data-position='top' data-tooltip='0%'>0</span> step(s) failed, <span class='strong tooltipped' data-position='top' data-tooltip='0%'>0</span> others
				</div>
			</div>
		</div>
		
	</div>
</div>

	<div class='subview-left left'>
		
		<div class='view-summary'>
			<h5>Tests</h5>
			<ul id='test-collection' class='test-collection'>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='1'>
					<div class='test-heading'>
						<span class='test-name'>testDetectJSError</span>
						<span class='test-time'>Mar 27, 2021 11:18:14 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:14 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:15 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+47ms</span>
</div>
	<div class='test-desc'>expected JS error </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>JavaScriptErrorPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:15 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='2'>
					<div class='test-heading'>
						<span class='test-name'>testDownloadFile</span>
						<span class='test-time'>Mar 27, 2021 11:18:16 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:16 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:21 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 5s+52ms</span>
</div>
	<div class='test-desc'>testDownloadFile </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>FileDownloadPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:21 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='3'>
					<div class='test-heading'>
						<span class='test-name'>testDragDropPage</span>
						<span class='test-time'>Mar 27, 2021 11:18:22 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:22 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:22 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+312ms</span>
</div>
	<div class='test-desc'>drag and drop page test </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>DragDropTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:22 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='4'>
					<div class='test-heading'>
						<span class='test-name'>testLoadNewText</span>
						<span class='test-time'>Mar 27, 2021 11:18:23 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:23 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:28 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 5s+156ms</span>
</div>
	<div class='test-desc'>testLoadNewText </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>DynamicLoadingPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:28 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='5'>
					<div class='test-heading'>
						<span class='test-name'>testHoverToSeeUserInfo</span>
						<span class='test-time'>Mar 27, 2021 11:18:29 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:29 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:30 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+379ms</span>
</div>
	<div class='test-desc'>mouse hover </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>MouseHoverPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:30 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='6'>
					<div class='test-heading'>
						<span class='test-name'>testUploadFile</span>
						<span class='test-time'>Mar 27, 2021 11:18:31 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:31 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:31 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+76ms</span>
</div>
	<div class='test-desc'>testUploadFile </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>FileUploadPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:31 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='7'>
					<div class='test-heading'>
						<span class='test-name'>testDynamicContent</span>
						<span class='test-time'>Mar 27, 2021 11:18:32 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:32 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:32 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+339ms</span>
</div>
	<div class='test-desc'>Test content changes with page reload. </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>DynamicContentPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:32 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='8'>
					<div class='test-heading'>
						<span class='test-name'>testEnabledTextField</span>
						<span class='test-time'>Mar 27, 2021 11:18:33 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:33 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:36 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 3s+244ms</span>
</div>
	<div class='test-desc'>testEnabledTextField </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>DynamicControlPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:36 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='9'>
					<div class='test-heading'>
						<span class='test-name'>testRemoveCheckBox</span>
						<span class='test-time'>Mar 27, 2021 11:18:37 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:37 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:37 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+78ms</span>
</div>
	<div class='test-desc'>testRemoveCheckBox </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>DynamicControlPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:37 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='10'>
					<div class='test-heading'>
						<span class='test-name'>testUnCheckedBox</span>
						<span class='test-time'>Mar 27, 2021 11:18:38 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:38 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:38 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+15ms</span>
</div>
	<div class='test-desc'>un-checked box test </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>CheckBoxTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:38 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='11'>
					<div class='test-heading'>
						<span class='test-name'>testCheckedBox</span>
						<span class='test-time'>Mar 27, 2021 11:18:39 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:39 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:39 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+17ms</span>
</div>
	<div class='test-desc'>checked box test </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>CheckBoxTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:39 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='12'>
					<div class='test-heading'>
						<span class='test-name'>testJSalert</span>
						<span class='test-time'>Mar 27, 2021 11:18:40 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:40 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:40 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+58ms</span>
</div>
	<div class='test-desc'>JS Alert Accept </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>JavaScriptAlertPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:40 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='13'>
					<div class='test-heading'>
						<span class='test-name'>testJSConfirm</span>
						<span class='test-time'>Mar 27, 2021 11:18:41 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:41 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:42 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+57ms</span>
</div>
	<div class='test-desc'>JS Alert Comfirm </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>JavaScriptAlertPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:42 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='14'>
					<div class='test-heading'>
						<span class='test-name'>testJSPrompt</span>
						<span class='test-time'>Mar 27, 2021 11:18:43 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:43 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:43 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+64ms</span>
</div>
	<div class='test-desc'>JS Alert Prompt </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>JavaScriptAlertPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:43 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='15'>
					<div class='test-heading'>
						<span class='test-name'>secondFirstOption</span>
						<span class='test-time'>Mar 27, 2021 11:18:44 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:44 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:44 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+65ms</span>
</div>
	<div class='test-desc'>drap down Option 2 test </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>DropDownPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:44 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='16'>
					<div class='test-heading'>
						<span class='test-name'>testFirstOption</span>
						<span class='test-time'>Mar 27, 2021 11:18:45 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:45 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:45 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+60ms</span>
</div>
	<div class='test-desc'>drap down Option 1 test </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>DropDownPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:45 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='17'>
					<div class='test-heading'>
						<span class='test-name'>testContextPage</span>
						<span class='test-time'>Mar 27, 2021 11:18:46 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:46 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:46 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+154ms</span>
</div>
	<div class='test-desc'>alert handle test </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>ContextMenuPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:46 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='18'>
					<div class='test-heading'>
						<span class='test-name'>testOpenNewTab</span>
						<span class='test-time'>Mar 27, 2021 11:18:47 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:47 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:47 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+127ms</span>
</div>
	<div class='test-desc'>new window handling </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>OpenNewTabPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:47 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='19'>
					<div class='test-heading'>
						<span class='test-name'>testScrollAndCheckMenuFloating</span>
						<span class='test-time'>Mar 27, 2021 11:18:48 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:48 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:48 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+21ms</span>
</div>
	<div class='test-desc'>testScrollAndCheckMenuFloating </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>FloatingMenuPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:48 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='20'>
					<div class='test-heading'>
						<span class='test-name'>testNotification</span>
						<span class='test-time'>Mar 27, 2021 11:18:49 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:49 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:49 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+158ms</span>
</div>
	<div class='test-desc'>Test notification Message. </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>NotificationMessageRenderedPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:49 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='21'>
					<div class='test-heading'>
						<span class='test-name'>testPageTitleTest</span>
						<span class='test-time'>Mar 27, 2021 11:18:50 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:50 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:50 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+6ms</span>
</div>
	<div class='test-desc'>get page title method </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>LoginPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:50 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='22'>
					<div class='test-heading'>
						<span class='test-name'>testLoginValidCreds</span>
						<span class='test-time'>Mar 27, 2021 11:18:51 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:51 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:52 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+249ms</span>
</div>
	<div class='test-desc'>valid username and password login </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>LoginPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:52 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='23'>
					<div class='test-heading'>
						<span class='test-name'>testLoginInvalidCreds</span>
						<span class='test-time'>Mar 27, 2021 11:18:53 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:53 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:53 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+250ms</span>
</div>
	<div class='test-desc'>invalid username and password login </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>LoginPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:53 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='24'>
					<div class='test-heading'>
						<span class='test-name'>testLoginInvalidCreds</span>
						<span class='test-time'>Mar 27, 2021 11:18:55 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:55 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:55 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+244ms</span>
</div>
	<div class='test-desc'>invalid username and password login </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>LoginPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:55 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='25'>
					<div class='test-heading'>
						<span class='test-name'>testLoginInvalidCreds</span>
						<span class='test-time'>Mar 27, 2021 11:18:56 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:56 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:56 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+237ms</span>
</div>
	<div class='test-desc'>invalid username and password login </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>LoginPageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:56 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
				
				
				<li class='test displayed active  pass' status='pass' bdd='false' test-id='26'>
					<div class='test-heading'>
						<span class='test-name'>testInputTextToIframe</span>
						<span class='test-time'>Mar 27, 2021 11:18:58 PM</span>
						<span class='test-status right pass'>pass</span>
					</div>
					<div class='test-content hide'>
<div class='test-time-info'>
	<span class='label start-time'>Mar 27, 2021 11:18:58 PM</span>
	<span class='label end-time'>Mar 27, 2021 11:18:58 PM</span>
	<span class='label time-taken grey lighten-1 white-text'>0h 0m 0s+187ms</span>
</div>
	<div class='test-desc'>iFrame test </div>
	<div class='test-attributes'>
			<div class='category-list'>
				<span class='category label white-text'>Suite</span>
				<span class='category label white-text'>IFramePageTest</span>
			</div>
	</div>
	<div class='test-steps'>
		<table class='bordered table-results'>
			<thead>
				<tr>
					<th>Status</th>
					<th>Timestamp</th>
					<th>Details</th>
				</tr>
			</thead>
			<tbody>
				<tr class='log' status='pass'>
					<td class='status pass' title='pass' alt='pass'><i class='material-icons'>check_circle</i></td>
					<td class='timestamp'>11:18:58 PM</td>
					<td class='step-details'>Test passed</td>
				</tr>
			</tbody>
		</table>
	</div>
					</div>
				</li>
			</ul>
		</div>
	</div>
	<!-- subview left -->

	<div class='subview-right left'>
		<div class='view-summary'>
			<h5 class='test-name'></h5>

			<div id='step-filters' class="right">
				<span class="blue-text" status="info" alt="info" title="info"><i class="material-icons">info_outline</i></span>
				<span class="green-text" status="pass" alt="pass" title="pass"><i class="material-icons">check_circle</i></span>
				<span class="red-text" status="fail" alt="fail" title="fail"><i class="material-icons">cancel</i></span>
				<span class="red-text text-darken-4" status="fatal" alt="fatal" title="fatal"><i class="material-icons">cancel</i></span>
				<span class="pink-text text-lighten-1" status="error" alt="error" title="error"><i class="material-icons">error</i></span>
				<span class="orange-text" alt="warning" status="warning" title="warning"><i class="material-icons">warning</i></span>
				<span class="teal-text" status="skip" alt="skip" title="skip"><i class="material-icons">redo</i></span>
				<span status="clear" alt="Clear filters" title="Clear filters"><i class="material-icons">clear</i></span>
			</div>
		</div>
	</div>
	<!-- subview right -->

</div>
<!-- test view -->
<div id='category-view' class='view hide'>

	<section id='controls'>
		<div class='controls grey lighten-4'>
			<!-- search -->
			<div class='chip transparent' alt='Search Tests' title='Search Tests'>
				<a href="#" class='search-div'>
					<i class='material-icons'>search</i> Search
				</a>
				
				<div class='input-field left hide'>
					<input id='search-tests' type='text' class='validate browser-default' placeholder='Search Tests...'>
				</div>
				
			</div>
			<!-- search -->
		</div>
	</section>

	<div class='subview-left left'>
		
		<div class='view-summary'>
			<h5>Categories</h3>
			<ul id='category-collection' class='category-collection'>
				
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>Suite</span>
						<span class='category-status right'>
							<span class='label pass'>26</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 26</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:14 PM</td>
										<td class='linked' test-id='1'>testDetectJSError</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:16 PM</td>
										<td class='linked' test-id='2'>testDownloadFile</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:22 PM</td>
										<td class='linked' test-id='3'>testDragDropPage</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:23 PM</td>
										<td class='linked' test-id='4'>testLoadNewText</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:29 PM</td>
										<td class='linked' test-id='5'>testHoverToSeeUserInfo</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:31 PM</td>
										<td class='linked' test-id='6'>testUploadFile</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:32 PM</td>
										<td class='linked' test-id='7'>testDynamicContent</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:33 PM</td>
										<td class='linked' test-id='8'>testEnabledTextField</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:37 PM</td>
										<td class='linked' test-id='9'>testRemoveCheckBox</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:38 PM</td>
										<td class='linked' test-id='10'>testUnCheckedBox</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:39 PM</td>
										<td class='linked' test-id='11'>testCheckedBox</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:40 PM</td>
										<td class='linked' test-id='12'>testJSalert</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:41 PM</td>
										<td class='linked' test-id='13'>testJSConfirm</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:43 PM</td>
										<td class='linked' test-id='14'>testJSPrompt</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:44 PM</td>
										<td class='linked' test-id='15'>secondFirstOption</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:45 PM</td>
										<td class='linked' test-id='16'>testFirstOption</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:46 PM</td>
										<td class='linked' test-id='17'>testContextPage</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:47 PM</td>
										<td class='linked' test-id='18'>testOpenNewTab</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:48 PM</td>
										<td class='linked' test-id='19'>testScrollAndCheckMenuFloating</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:49 PM</td>
										<td class='linked' test-id='20'>testNotification</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:50 PM</td>
										<td class='linked' test-id='21'>testPageTitleTest</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:51 PM</td>
										<td class='linked' test-id='22'>testLoginValidCreds</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:53 PM</td>
										<td class='linked' test-id='23'>testLoginInvalidCreds</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:55 PM</td>
										<td class='linked' test-id='24'>testLoginInvalidCreds</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:56 PM</td>
										<td class='linked' test-id='25'>testLoginInvalidCreds</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:58 PM</td>
										<td class='linked' test-id='26'>testInputTextToIframe</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>JavaScriptErrorPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:14 PM</td>
										<td class='linked' test-id='1'>testDetectJSError</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>FileDownloadPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:16 PM</td>
										<td class='linked' test-id='2'>testDownloadFile</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>DragDropTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:22 PM</td>
										<td class='linked' test-id='3'>testDragDropPage</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>DynamicLoadingPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:23 PM</td>
										<td class='linked' test-id='4'>testLoadNewText</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>MouseHoverPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:29 PM</td>
										<td class='linked' test-id='5'>testHoverToSeeUserInfo</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>FileUploadPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:31 PM</td>
										<td class='linked' test-id='6'>testUploadFile</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>DynamicContentPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:32 PM</td>
										<td class='linked' test-id='7'>testDynamicContent</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>DynamicControlPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>2</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 2</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:33 PM</td>
										<td class='linked' test-id='8'>testEnabledTextField</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:37 PM</td>
										<td class='linked' test-id='9'>testRemoveCheckBox</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>CheckBoxTest</span>
						<span class='category-status right'>
							<span class='label pass'>2</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 2</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:38 PM</td>
										<td class='linked' test-id='10'>testUnCheckedBox</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:39 PM</td>
										<td class='linked' test-id='11'>testCheckedBox</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>JavaScriptAlertPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>3</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 3</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:40 PM</td>
										<td class='linked' test-id='12'>testJSalert</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:41 PM</td>
										<td class='linked' test-id='13'>testJSConfirm</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:43 PM</td>
										<td class='linked' test-id='14'>testJSPrompt</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>DropDownPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>2</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 2</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:44 PM</td>
										<td class='linked' test-id='15'>secondFirstOption</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:45 PM</td>
										<td class='linked' test-id='16'>testFirstOption</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>ContextMenuPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:46 PM</td>
										<td class='linked' test-id='17'>testContextPage</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>OpenNewTabPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:47 PM</td>
										<td class='linked' test-id='18'>testOpenNewTab</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>FloatingMenuPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:48 PM</td>
										<td class='linked' test-id='19'>testScrollAndCheckMenuFloating</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>NotificationMessageRenderedPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:49 PM</td>
										<td class='linked' test-id='20'>testNotification</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>LoginPageTest</span>
						<span class='category-status right'>
							<span class='label pass'>5</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 5</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:50 PM</td>
										<td class='linked' test-id='21'>testPageTitleTest</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:51 PM</td>
										<td class='linked' test-id='22'>testLoginValidCreds</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:53 PM</td>
										<td class='linked' test-id='23'>testLoginInvalidCreds</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:55 PM</td>
										<td class='linked' test-id='24'>testLoginInvalidCreds</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
									<tr>
										<td>Mar 27, 2021 11:18:56 PM</td>
										<td class='linked' test-id='25'>testLoginInvalidCreds</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>
				<li class='category displayed active'>
					<div class='category-heading'>
						<span class='category-name'>IFramePageTest</span>
						<span class='category-status right'>
							<span class='label pass'>1</span>
						</span>
					</div>
					<div class='category-content hide'>
						<div class='category-status-counts'>
							<span class='label green accent-4 white-text'>Passed: 1</span>
							
							
						</div>
					
						<div class='category-tests'>
							<table class='bordered table-results'>
								<thead>
									<tr>
										<th>Timestamp</th>
										<th>TestName</th>
										<th>Status</th>
									</tr>
								</thead>
								<tbody>
									<tr>
										<td>Mar 27, 2021 11:18:58 PM</td>
										<td class='linked' test-id='26'>testInputTextToIframe</td>
										<td><span class='test-status pass'>pass</span></td>
									</tr>
								</tbody>
							</table>
						</div>
					</div>
				</li>

			</ul>
		</div>
	</div>

	<div class='subview-right left'>
		<div class='view-summary'>
			<h5 class='category-name'></h5>
		</div>
	</div>
</div>
<!-- category view -->
<!-- exception view -->
<div id='dashboard-view' class='view hide'>
	<div class='card-panel transparent np-v'>
		<h5>Dashboard</h5>

		<div class='row'>
			<div class='col s2'>
				<div class='card-panel r'>
					Tests
					<div class='panel-lead'>26</div>
				</div>
			</div>
			<div class='col s2'>
				<div class='card-panel r'>
					Steps
					<div class='panel-lead'>26</div>
				</div>
			</div>
			<div class='col s2'>
				<div class='card-panel r'>
					Start
					<div class='panel-lead'>Mar 27, 2021 11:18:13 PM</div>
				</div>
			</div>
			<div class='col s2'>
				<div class='card-panel r'>
			 		End
			 		<div class='panel-lead'>Mar 27, 2021 11:18:58 PM</div>
				</div>
			</div>
			<div class='col s2'>
				<div class='card-panel r'>
					Time Taken
					<div class='panel-lead'>0h 0m 45s+962ms</div>
				</div>
			</div>
			<div class='col s6'>
				<div class='card-panel dashboard-categories'>
					<span class='right label cyan white-text'>Categories</span><p>&nbsp;</p>
					
					<table>
						<tr>
							<th>Name</th>
							<th>Passed</th>
							<th>Failed</th>
							<th>Others</th>
							<th>Passed %</th>
						</tr>
						<tr>
							<td>Suite</td>
							<td>26</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>JavaScriptErrorPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>FileDownloadPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>DragDropTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>DynamicLoadingPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>MouseHoverPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>FileUploadPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>DynamicContentPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>DynamicControlPageTest</td>
							<td>2</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>CheckBoxTest</td>
							<td>2</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>JavaScriptAlertPageTest</td>
							<td>3</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>DropDownPageTest</td>
							<td>2</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>ContextMenuPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>OpenNewTabPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>FloatingMenuPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>NotificationMessageRenderedPageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>LoginPageTest</td>
							<td>5</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
						<tr>
							<td>IFramePageTest</td>
							<td>1</td>
							<td>0</td>
							<td>0</td>
							<td>
									100%
							</td>
						</tr>
					</table>
				</div>
			</div>
		</div>
	</div>
</div>
<!-- dashboard view -->
<!-- testrunner-logs view -->
		</div>
		<!-- container -->

		<script>
			var statusGroup = {
				passParent: 26,
				failParent: 0,
				fatalParent: 0,
				errorParent: 0,
				warningParent: 0,
				skipParent: 0,
				exceptionsParent: 0,
				
				passChild: 26,
				failChild: 0,
				fatalChild: 0,
				errorChild: 0,
				warningChild: 0,
				skipChild: 0,
				infoChild: 0,
				exceptionsChild: 0,
				
				passGrandChild: 0,
				failGrandChild: 0,
				fatalGrandChild: 0,
				errorGrandChild: 0,
				warningGrandChild: 0,
				skipGrandChild: 0,
				infoGrandChild: 0,
				exceptionsGrandChild: 0,
			};
		</script>
		
			<script src='https://cdn.rawgit.com/anshooarora/extentreports-java/fca20fb7653aade98810546ab96a2a4360e3e712/dist/js/extent.js' type='text/javascript'></script>
		
		
 		<script type='text/javascript'>
 		</script>
	</body>
	
</html>
```
