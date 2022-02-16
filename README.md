# longrun
A simple utility allowing long running tasks to be executed without blocking

**install**
pip install longrun

**example usage**

import longrun

async def my_task_launcher(task, *args, **kwargs):
  result = await longrun.slow_exec(task, *args, **kwargs)
  return result
