checkmk
=======

Checkmk is an awk parser for Check unit testing framework (latest 9.10 version). I updated it to support more directives.

	#test-loop(start, end) test_name -> tcase_add_loop_test(tcase, test_name ,start ,end);
	#test-exit(exit_value) test_name -> tcase_add_exit_test(tcase, test_name, exit_value);
	#test-signal(signal) test_name -> tcase_add_test_raise_signal(tcase, test_name ,exit_value);
	#test-loop-exit(exit_value, start, end) test_name -> tcase_add_loop_exit_test(tcase, test_name ,exit_value, start ,end);
	#test-loop-signal(signal, start, end) test_name -> tcase_add_loop_test_raise_signal(tcase, test_name, signal, start, end);


All directives work with any amount of spaces / tabs combination between parentheses and arguments

Installation
=======

You can copy paste the checkmk folder to the current check 9.10 trunk directory and run the tests as well.
If you don't want to compile the framework, look in the standalone folder for a ready-to-use version