BlockPos
********

.. default-domain:: csharp

.. class:: BlockPos

	.. property:: int x { get; set; }
	
		Local x coordinate.
	
	.. property:: int y { get; set; }
	
		local y coordinate.
	
	.. property:: int z { get; set; }
	
		local z coordinate.
		
	.. property:: ChunkPos chunkPos { get; set; }
	
		The chunk this block is located in.
		
	.. property:: static BlockPos zero { get; }
	
		Shorthand for writing BlockPos(0, 0, 0).
	
	.. property:: static BlockPos up { get; }
	
		Shorthand for writing BlockPos(0, 1, 0).
	
	.. property:: static BlockPos down { get; }
	
		Shorthand for writing BlockPos(0, -1, 0).
	
	.. property:: static BlockPos north { get; }
	
		Shorthand for writing BlockPos(0, 0, 1).
	
	.. property:: static BlockPos south { get; }
	
		Shorthand for writing BlockPos(0, 0, -1).
	
	.. property:: static BlockPos east { get; }
	
		Shorthand for writing BlockPos(1, 0, 0).
	
	.. property:: static BlockPos west { get; }
	
		Shorthand for writing BlockPos(-1, 0, 0).

	.. method:: BlockPos (int x, int y, int z, ChunkPos chunkPos = ChunkPos.zero)
	
		Creates a new :type:`BlockPos` using explicit x, y, and z coordinates inside a ChunkPos.
	
	.. method:: public int GetWorldX ()
	
		Returns global x coordinate.
	
	.. method:: public int GetWorldY ()
	
		Returns global y coordinate.
	
	.. method:: public int GetWorldZ ()
	
		Returns global z coordinate.
	
	.. method:: int Mod (int x, int m)
	
		The default C# modulus operator % returns negative numbers for negative input, which is undesirable.
	
	.. method:: void Correct ()
	
		This corrects overflown coordinates, appropriately shifting chunkPos and clamping x, y, and z.