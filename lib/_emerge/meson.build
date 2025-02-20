AbstractEbuildProcess_py = configure_file(
    input : 'AbstractEbuildProcess.py',
    output : 'AbstractEbuildProcess.py',
    configuration : {'IPC' : get_option('ipc')}
)

create_depgraph_params_py = configure_file(
    input : 'create_depgraph_params.py',
    output : 'create_depgraph_params.py',
    configuration : {'DYN_DEPS_DEFAULT' : get_option('gentoo-dev') ? 'n' : 'y'}
)

py.install_sources(
    [
        'AbstractDepPriority.py',
        AbstractEbuildProcess_py,
        'AbstractPollTask.py',
        'AsynchronousLock.py',
        'AsynchronousTask.py',
        'AtomArg.py',
        'BinpkgEnvExtractor.py',
        'BinpkgExtractorAsync.py',
        'BinpkgFetcher.py',
        'BinpkgPrefetcher.py',
        'BinpkgVerifier.py',
        'Binpkg.py',
        'BlockerCache.py',
        'BlockerDB.py',
        'BlockerDepPriority.py',
        'Blocker.py',
        'CompositeTask.py',
        'DepPriorityNormalRange.py',
        'DepPrioritySatisfiedRange.py',
        'DepPriority.py',
        'DependencyArg.py',
        'Dependency.py',
        'EbuildBinpkg.py',
        'EbuildBuildDir.py',
        'EbuildBuild.py',
        'EbuildExecuter.py',
        'EbuildFetcher.py',
        'EbuildFetchonly.py',
        'EbuildIpcDaemon.py',
        'EbuildMerge.py',
        'EbuildMetadataPhase.py',
        'EbuildPhase.py',
        'EbuildProcess.py',
        'EbuildSpawnProcess.py',
        'FakeVartree.py',
        'FifoIpcDaemon.py',
        'JobStatusDisplay.py',
        'MergeListItem.py',
        'MetadataRegen.py',
        'MiscFunctionsProcess.py',
        'PackageArg.py',
        'PackageMerge.py',
        'PackagePhase.py',
        'PackageUninstall.py',
        'PackageVirtualDbapi.py',
        'Package.py',
        'PipeReader.py',
        'PollScheduler.py',
        'ProgressHandler.py',
        'RootConfig.py',
        'Scheduler.py',
        'SequentialTaskQueue.py',
        'SetArg.py',
        'SpawnProcess.py',
        'SubProcess.py',
        'TaskSequence.py',
        'Task.py',
        'UninstallFailure.py',
        'UnmergeDepPriority.py',
        'UseFlagDisplay.py',
        'UserQuery.py',
        'actions.py',
        'chk_updated_cfg_files.py',
        'clear_caches.py',
        'countdown.py',
        create_depgraph_params_py,
        'create_world_atom.py',
        'depgraph.py',
        'emergelog.py',
        'getloadavg.py',
        'help.py',
        'is_valid_package_atom.py',
        'main.py',
        'post_emerge.py',
        'search.py',
        'show_invalid_depstring_notice.py',
        'stdout_spinner.py',
        'unmerge.py',
        '_find_deep_system_runtime_deps.py',
        '_flush_elog_mod_echo.py',
        '__init__.py',
    ],
    subdir : '_emerge',
    pure : false
)

subdir('resolver')
