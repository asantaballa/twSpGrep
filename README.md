twSpGrep
========

Simple stored proc searcher for SQL server which displays the lines found rather then the procs found.

Sample output from: Exec #twSpGrep 'raiserror'

Name                        LineNumber    Line
dt_displayoaerror                   16      raiserror (@vchOutput,16,-1)
dt_getobjwithprop                   12    raiserror('Must specify a property name.',-1,-1)
dt_getobjwithprop_u                 12    raiserror('Must specify a property name.',-1,-1)
dt_vcsenabled                       15        if @iReturn <> 0 raiserror('', 16, -1) /* Can't Load Helper DLLC */
sp_alterlineitem                    24    RAISERROR ('Invalid ARG', 16, 1)
sp_alterlineitem                    40    RAISERROR ('lineitem does not exist or you do not have permission.', 16, 1);
sp_createlineitem                   20    RAISERROR (N'E_INVALIDARG', 16, 1);
sp_createlineitem                   39     RAISERROR (N'E_INVALIDARG', 16, 1);
sp_createlineitem                   48    RAISERROR ('The name is already used.', 16, 1);
sp_droplineitem                     19    RAISERROR ('Invalid value', 16, 1);
sp_droplineitem                     33    RAISERROR ('lineitem does not exist or you do not have permission.', 16, 1)
sp_helplineitemdefinition           19    RAISERROR (N'E_INVALIDARG', 16, 1);
sp_helplineitemdefinition           33    RAISERROR ('lineitem does not exist or you do not have permission.', 16, 1);
sp_renamelineitem                   22    RAISERROR ('Invalid value', 16, 1);
sp_renamelineitem                   38    RAISERROR ('lineitem does not exist or you do not have permission.', 16, 1)
sp_renamelineitem                   52    RAISERROR ('The name is already used.', 16, 1);

