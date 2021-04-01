currently crashing at 100% world gen with this

Unhandled Exception C0000005 (EXCEPTION_ACCESS_VIOLATION) at address 0x00007FF6AAD0CB1D

Stack Trace: 
  1    imperator_D_opt.exe      CCountryFamily::ValidateAndGenerateDesiredAmountOfFamilies (country_families.cpp: 366)
  2    imperator_D_opt.exe      CCountryFamily::PickFamily (country_families.cpp: 329)
  3    imperator_D_opt.exe      CCharacterManager::CreateRandomCharacter (character_manager.cpp: 230)
  4    imperator_D_opt.exe      CCharacterManager::CreateRandomCharacter (character_manager.cpp: 143)
  5    imperator_D_opt.exe      CMercenary::CreateNewLeader (mercenary.cpp: 329)
  6    imperator_D_opt.exe      CMercenaryManager::MakeMercenaryInternal (mercenary_manager.cpp: 379)
  7    imperator_D_opt.exe      CMercenaryManager::MakeMercenary (mercenary_manager.cpp: 417)
  8    imperator_D_opt.exe      CMercenaryManager::AddNewMercenaries (mercenary_manager.cpp: 359)
  9    imperator_D_opt.exe      CMercenaryManager::UpdateTurnTick (mercenary_manager.cpp: 75)
  10   imperator_D_opt.exe      InitializeGameStateFromBookmark (gamestate.cpp: 1811)
  11   imperator_D_opt.exe      CGenerateFromBookmarkIdlerLogic::GenerateFromBookmarkTask (generatefrombookmarkidlerlogic.cpp: 73)
  12   imperator_D_opt.exe      boost::detail::function::void_function_obj_invoker0<boost::_bi::bind_t<void,boost::_mfi::mf0<void,CGenerateFromBookmarkIdlerLogic>,boost::_bi::list1<boost::_bi::value<CGenerateFromBookmarkIdlerLogic *> > >,void>::invoke (function_template.hpp: 159)
  13   imperator_D_opt.exe      boost::function0<void>::operator() (function_template.hpp: 765)
  14   imperator_D_opt.exe      CPdxTaskScheduler::RunTasks (pdx_task_scheduler.cpp: 449)
  15   imperator_D_opt.exe      CPdxTaskScheduler::Run (pdx_task_scheduler.cpp: 592)
  16   imperator_D_opt.exe      CTaskThread::Run (pdx_task_scheduler.cpp: 107)
  17   imperator_D_opt.exe      CPdxCrashReporter::ThreadCallbackWrapper (pdx_crashreport.cpp: 291)
  18   imperator_D_opt.exe      ThreadFunc (pdx_thread_cxx11.cpp: 50)
  19   imperator_D_opt.exe      std::thread::_Invoke<std::tuple<void * (__cdecl*)(void * (__cdecl*)(void *),void *,char const *),void * (__cdecl*)(void *),void *,char const *>,0,1,2,3> (thread: 44)
  20   imperator_D_opt.exe      thread_start<unsigned int (__cdecl*)(void *),1> (thread.cpp: 97)
  21   KERNEL32.DLL             BaseThreadInitThunk (+ 20)
  22   ntdll.dll                RtlUserThreadStart (+ 33)
  23   ntdll.dll                RtlUserThreadStart (+ 33)
