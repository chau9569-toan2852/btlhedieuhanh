
					
Project 1: Thread 
--------------------------------------------------------------------------------------------------------
LE BAO CHAU (LEADER)----20209569--------Alarm
NGUYEN VAN TOAN---------20172852--------Priority Donation
NGUYEN NGOC HUY---------20172606--------Advanced Scheduler
--------------------------------------------------------------------------------------------------------
* In src/device
	timer.c
		- addition: 	timer_interrupt()
		- modification: timer_sleep()
* In src/threads
	thread.c
		- addition: 	thread_create()
		- implementation:checkInvoke(), thread_cmp_priority(), thread_donate-priority(), 					thread_hold_lock(), thread_remove_lock(), lock_cmp_priority(), 					thread_update_priority()
		- modification:	thread_unblock(), thread_yield(), thread_set_priority(), init_thread()
	thread.h
		- addition:	struct thread
		- declaration:	checkInvoke(), thread_remove_lock(), thread_cmp_priority(), 					thread_donate-priority, thread_hold_lock(), thread_update_priority(), 					lock_cmp_priority()
		- inclusion:
	synch.c
		- addition: 	sema_down(), sema_up(), lock_release(), cond-signal(), cond_signal()
		- implementation:cond_sema_cmp_priority()
		- modification:	lock_acquire()
	synch.h
		- addition: 	struct lock 
		- declaration:	cond_sema_cmp_priority()
--------------------------------------------------------------------------------------------------------
GHVD: TS. Pham Van Tien
