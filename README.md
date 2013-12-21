checkmk
=======

Checkmk is an awk parser for Check unit testing framework. I updated it to support more directives.
Update: Code is now included upstream!

	#test-loop(start, end) test_name -> tcase_add_loop_test(tcase, test_name ,start ,end);
	#test-exit(exit_value) test_name -> tcase_add_exit_test(tcase, test_name, exit_value);
	#test-signal(signal) test_name -> tcase_add_test_raise_signal(tcase, test_name ,exit_value);
	#test-loop-exit(exit_value, start, end) test_name -> tcase_add_loop_exit_test(tcase, test_name ,exit_value, start ,end);
	#test-loop-signal(signal, start, end) test_name -> tcase_add_loop_test_raise_signal(tcase, test_name, signal, start, end);


All directives work with any amount of spaces / tabs combination between parentheses and arguments.
