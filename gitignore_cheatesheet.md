Pattern                                         Explanation/Matches                                                                Examples
**/logs                                          You can prepend a pattern with a double asterisk                                   logs/debug.log
                                                 to match directories anywhere in the repository.                                   logs/monday/foo.bar
                                                 
                                                 
 logs/                                          Appending a slash indicates the pattern is a directory.                                logs/debug.log
                                                 The entire contents of any directory in the repository matching                       logs/latest/foo.bar      
                                                 that name – including all of its files and subdirectories – will be ignored            build/logs/foo.bar
                                                                                                                                        build/logs/latest/debug.log
                                                                                                                                        
 
 
logs/**/debug.log                               A double asterisk matches zero or more directories.                                     logs/debug.log 
                                                                                                                                        logs/monday/debug.log
                                                                                                                                        logs/monday/pm/debug.log




debug.log                                    By default, patterns match files in any directory                                         debug.log
                                                                                                                                       logs/debug.log 



debug?.log                                     A question mark matches exactly one character.                                           debug0.log
                                                                                                                                       debugg.log
                                                                                                                                       but not
                                                                                                                                       debug10.log


