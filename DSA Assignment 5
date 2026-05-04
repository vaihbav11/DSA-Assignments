 class Solution:
    def numIslands(self, grid):
        if not grid:
            return 0

        count = 0 

        def dfs(r, c):
            # out of bounds or water or visited — stop
            if r < 0 or r >= len(grid) or c < 0 or c >= len(grid[0]) or grid[r][c] == '0':
                return
            grid[r][c] = '0'  # mark visited by sinking the land
            dfs(r+1, c) 
            dfs(r-1, c)
            dfs(r, c+1)
            dfs(r, c-1)

        for r in range(len(grid)):
            for c in range(len(grid[0])):
                if grid[r][c] == '1':
                    count += 1  # new island found
                    dfs(r, c)   # sink the whole island

        return count
